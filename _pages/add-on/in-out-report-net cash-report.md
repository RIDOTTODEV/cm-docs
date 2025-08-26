---
title: "In-out Net Cash Summary Report"
parent: "Add-on"
layout: single
nav_order: 8
permalink: /add-on/in-out-net-cash-summary-report/
read_time: true
toc: true
toc_sticky: true
categories:
  - Add-on
tags:
  - Report
  - Player
---

## In-out Net Cash Summary Report

Belirtilen tarih aralığında oyuncuları kategori (PlayerCategory) bazında gruplayarak; LG sonucu, Slot sonucu, harcama (expense), doküman ve net nakit (Net Cash) özetlerini üretir.

---

## Özellikler ve Açıklamalar

- **PlayerCategory**: Grup anahtarı. Oyuncunun kategorisi (ör. Local/Foreign vb.).
- **PlayerCount**: İlgili kategorideki ziyaret sayıları toplamı.
    - Kaynak: `GetPlayerVisitCount` → oyuncu bazında `Count`
    - Formül (kategori için): `Count toplamı`
- **TotalLgResult**: LG tarafındaki toplam sonuç.
    - Kaynak: `GetLgInfoForNetCash` → oyuncu bazında `LgResult`
    - Formül (kategori için): `LgResult toplamı`
- **TotalSlotResult**: Slot tarafındaki toplam sonuç.
    - Kaynak: `GetSlotInfoForNetCash` → oyuncu bazında `SlotResult`
    - Formül (kategori için): `SlotResult toplamı`
- **TotalResult**: Toplam oyun sonucu.
    - Formül: `TotalLgResult + TotalSlotResult`
- **GamingExpense**: Toplam oyun harcaması(Disc+com vb.)
    - Kaynak: `GetPlayerExpenseAndDocument` → oyuncu bazında `TotalExpense`
    - Formül (kategori için): `TotalExpense toplamı`
- **Documents**: Oyuncularla ilişkili belge toplamları (çek+senet vb.).
    - Kaynak: `GetPlayerExpenseAndDocument` → oyuncu bazında `TotalDocuments`
    - Formül (kategori için): `TotalDocuments toplamı`
- **GamingLoss**: Harcama dahil oyun kaybı göstergesi.
    - Formül: `TotalLgResult + TotalSlotResult + GamingExpense`
- **NetCash**: Net nakit.
    - Formül: `TotalResult - (GamingExpense + Documents)`
    - Açıklama: Oyun sonuçlarından harcama ve belgeler düşülür.

---

## Girdi

- **StartDate / EndDate**: Veri aralığı.
- **BalanceCurrencyId**: Tutarların çevirildiği para birimi.

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

- Her kayıt bir oyuncu kategorisine ait özetleri içerir. Çıktı, `NetCashSummaryReportOutput` listesi olarak döner.

Örnek cevap şeması:

```json
[
  {
    "playerCategory": "Local",
    "playerCount": 120,
    "totalLgResult": -25000.0,
    "totalSlotResult": -40000.0,
    "totalResult": -65000.0,
    "gamingExpense": 9000.0,
    "documents": 3000.0,
    "gamingLoss": -56000.0,
    "netCash": -77000.0
  }
]
```

---

## Notlar

- Tüm tutarlar, `balanceCurrencyId` ye çevrilmiştir.
- Gruplama anahtarı yalnızca `PlayerCategory`’dir; alanlar kategori içindeki oyuncu bazlı değerlerin toplamıdır.
- `PlayerCount`, kişi sayısı değil; ziyaret sayıları toplamıdır (oyuncu bazında `Count` değerlerinin toplamı).