---
title: "In-out Detailed In/Out Report"
parent: "Add-on"
layout: single
nav_order: 5
permalink: /add-on/in-out-detailed-inout-report/
read_time: true
toc: true
toc_sticky: true
categories:
  - Add-on
tags:
  - Report
  - Player
---

## In-out Detailed In/Out Report

Belirtilen tarih aralığında oyuncular için kasa (In/Out), Live Game (LG) ve Slot verilerini birleştirerek ayrıntılı bir In/Out raporu oluşturur.
---

## Features and Descriptions
- **PlayerId / PlayerName / PlayerCategory / PlayerClass**: Oyuncu kimlik ve sınıflandırma bilgileri.
- **CreditIn**: Kasa kredi açılışları toplamı. Kaynak: `GetPlayerInOuts` (pi.CreditIn).
- **CreditOut**: Kasa kredi geri ödemeleri toplamı. Kaynak: `GetPlayerInOuts` (pi.CreditOut).
- **DepositIn**: Kasa deposit girişleri toplamı. Kaynak: `GetPlayerInOuts` (pi.DepositIn).
- **DepositOut**: Kasa deposit çıkışları toplamı. Kaynak: `GetPlayerInOuts` (pi.DepositOut).
- **CreditCardIn**: Kredi kartı ile yapılan kasa girişleri toplamı. Kaynak: `GetPlayerInOuts` (pi.CreditCardIn).
- **CreditCardOut**: Kredi kartı ile yapılan kasa çıkışları toplamı. Kaynak: `GetPlayerInOuts` (pi.CreditCardOut).
- **CashIn**: Kasa nakit girişleri toplamı (chip dışı nakit akışlar dahil olabilir). Kaynak: `GetPlayerInOuts` (pi.CashIn).
- **CashOut**: Kasa nakit çıkışları toplamı (chip dışı nakit çıkışlar dahil olabilir). Kaynak: `GetPlayerInOuts` (pi.CashOut).
- **TableDrop**: Masalarda gerçekleşen toplam drop (kasa tarafında görülen toplam). Kaynak: `GetPlayerInOuts` (pi.TableDrop).
- **SlotResult**: Slot toplam sonuç (kazanç/kayıp). Kaynak: `GetSlotWinLoss` (sl.SlotResult).
- **ComplimentaryLiveGameIn**: LG complimentary girişleri toplamı. Kaynak: `GetPlayerInOuts` (pi.ComplimentaryLiveGameIn).
- **ComplimentaryLiveGameOut**: LG complimentary çıkışları toplamı. Kaynak: `GetPlayerInOuts` (pi.ComplimentaryLiveGameOut).
- **ComplimentarySlotIn**: Slot complimentary girişleri toplamı. Kaynak: `GetPlayerInOuts` (pi.ComplimentarySlotIn).
- **ComplimentarySlotOut**: Slot complimentary çıkışları toplamı. Kaynak: `GetPlayerInOuts` (pi.ComplimentarySlotOut).
- **LgCashDrop**: LG masalarında nakit drop toplamı. Kaynak: `GetPlayerLgInfo` (lg.CashDrop).
- **LgChipDrop**: LG masalarında plaque drop toplamı. Kaynak: `GetPlayerPlaqueDrops` (oyuncu bazında `PlaqueDrop` toplamı).
- **LgTotalDrop**: LG toplam drop.
    - Formül: `LgCashDrop + LgChipDrop`
- **LgTotalOut**: LG tarafındaki toplam out. Kaynak: `GetPlayerLgInfo` (lg.TotalOut).
- **LgResult**: LG oyun sonucu. Kaynak: `GetPlayerLgInfo` (lg.Result).

---

## Input

- **StartDate / EndDate**: Tarih aralığı
- **BalanceCurrencyId**: Sonuçların gösterileceği para birimi

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

- Her kayıt bir oyuncunun ayrıntılı In/Out verilerini içerir. Çıktı, `ReportDetailedInOutOutput` listesi olarak döner.

Örnek cevap şeması:

```json
[
  {
    "playerId": 1,
    "playerName": "Ridotto Admin",
    "playerCategory": "Local",
    "playerClass": "A",
    "creditIn": 5000.0,
    "creditOut": 3000.0,
    "depositIn": 2000.0,
    "depositOut": 0.0,
    "creditCardIn": 1500.0,
    "creditCardOut": 200.0,
    "cashIn": 1000.0,
    "cashOut": 300.0,
    "tableDrop": 2500.0,
    "slotResult": -400.0,
    "complimentaryLiveGameIn": 100.0,
    "complimentaryLiveGameOut": 50.0,
    "complimentarySlotIn": 80.0,
    "complimentarySlotOut": 40.0,
    "lgCashDrop": 1800.0,
    "lgChipDrop": 700.0,
    "lgTotalDrop": 2500.0,
    "lgTotalOut": 2100.0,
    "lgResult": -400.0
  }
]
```

---

## Notes

- Tüm tutarlar, `balanceCurrencyId` çevrilmiştir.
- LG ve Slot metrikleri birleştirilirken tarih filtreleri StartDate–EndDate aralığına uygulanır.