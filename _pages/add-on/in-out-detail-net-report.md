---
title: "In-out Detailed Net Report"
parent: "Add-on"
layout: single
nav_order: 6
permalink: /add-on/in-out-detailed-net-report/
read_time: true
toc: true
toc_sticky: true
categories:
  - Add-on
tags:
  - Report
  - Player
---

## In-out Detailed Net Report

`GetReportDetailInOut` çıktısını oyuncu bazında özetleyerek net kalemleri ve sonuçları döndürür.

---

## Özellikler ve Açıklamalar

- **PlayerId / PlayerName / PlayerCategory / PlayerClass**: Oyuncu kimlik ve sınıflandırma bilgileri.
- **Credit**: Net kredi.
  - Formül: `CreditOut toplamı - CreditIn toplamı`
  - Açıklama: Kredi geri ödemeleri toplamından kredi açılışları toplamı çıkarılır.
- **Deposit**: Net deposit.
  - Formül: `DepositOut toplamı - DepositIn toplamı`
  - Açıklama: Deposit çıkışları toplamından deposit girişleri toplamı çıkarılır.
- **CreditCard**: Net kredi kartı.
  - Formül: `CreditCardOut toplamı - CreditCardIn toplamı`
  - Açıklama: Kredi kartı çıkışları toplamından kredi kartı girişleri toplamı çıkarılır.
- **Cash**: Net nakit.
  - Formül: `CashOut toplamı - CashIn toplamı`
  - Açıklama: Nakit çıkışları toplamından nakit girişleri toplamı çıkarılır.
- **TableDrop**: Masalardaki toplam drop.
  - Formül: `TableDrop toplamı`
  - Açıklama: Tüm günlerdeki table drop değerleri toplanır.
- **SlotResult**: Slot toplam sonuç.
  - Formül: `SlotResult toplamı`
  - Açıklama: Tüm günlerdeki slot result değerleri toplanır.
- **ComplimentaryLiveGame**: Net LG complimentary.
  - Formül: `ComplimentaryLiveGameOut toplamı - ComplimentaryLiveGameIn toplamı`
  - Açıklama: LG complimentary çıkışları toplamından girişleri toplamı çıkarılır.
- **ComplimentarySlot**: Net Slot complimentary.
  - Formül: `ComplimentarySlotOut toplamı - ComplimentarySlotIn toplamı`
  - Açıklama: Slot complimentary çıkışları toplamından girişleri toplamı çıkarılır.
- **PlaqueDrop**: LG masalarında plaque drop toplamı.
  - Formül: `LgChipDrop toplamı`
  - Açıklama: Tüm günlerdeki plaque drop değerleri toplanır.
- **LgTotalOut**: LG tarafındaki toplam out.
  - Formül: `LgTotalOut toplamı`
  - Açıklama: Tüm günlerdeki LG total out değerleri toplanır.
- **LgResult**: LG oyun sonucu.
  - Formül: `LgResult toplamı`
  - Açıklama: Tüm günlerdeki LG result değerleri toplanır.

---

## Girdi

- **StartDate / EndDate**: Tarih aralığı
- **BalanceCurrencyId**: Sonuçların gösterileceği para birimi.

Örnek istek modeli:

```json
{
  "startDate": "2025-01-01",
  "endDate": "2025-01-31",
  "balanceCurrencyId": 2
}
```

---

## Çıktı

- Her kayıt bir oyuncunun net özet kalemlerini içerir. Çıktı, `ReportDetailedNetOutput` listesi olarak döner.

Örnek cevap şeması:

```json
[
  {
    "playerId": 1,
    "playerName": "Ridotto Admin",
    "playerCategory": "Local",
    "playerClass": "A",
    "credit": -2000.0,
    "deposit": -2000.0,
    "creditCard": -1300.0,
    "cash": -700.0,
    "tableDrop": 2500.0,
    "slotResult": -400.0,
    "complimentaryLiveGame": -50.0,
    "complimentarySlot": -40.0,
    "plaqueDrop": 700.0,
    "lgTotalOut": 2100.0,
    "lgResult": -400.0
  }
]
```

---

## Notlar

- Tüm tutarlar, detay kaynaklarında `balanceCurrencyId` ye çevrilmiştir.
- Hesaplamalar oyuncu bazında grup toplamları ile yapılır.
- Net değerler (Credit, Deposit, CreditCard, Cash, ComplimentaryLiveGame, ComplimentarySlot) çıkış - giriş formülü ile hesaplanır.
- Toplam değerler (TableDrop, SlotResult, PlaqueDrop, LgTotalOut, LgResult) sadece toplama işlemi ile hesaplanır.
- Bu rapor, `GetReportDetailInOut` metodunun çıktısını özetleyerek oyuncu başına tek satır net sonuç üretir.