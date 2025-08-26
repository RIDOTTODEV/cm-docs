---
title: "In-out Filtered Report"
parent: "Add-on"
layout: single
nav_order: 4
permalink: /add-on/in-out-filtered-report/
read_time: true
toc: true
toc_sticky: true
categories:
  - Add-on
tags:
  - Report
  - Player
---

## In-out Filtered Report

Belirtilen tarih aralığı için oyuncu bazında Slot ve Live Game (LG) verilerini birleştirerek filtrelenmiş özet bir rapor üretir.

---

## Özellikler ve Açıklamalar

- **PlayerId / PlayerName / PlayerCategory / PlayerClass / PlayerCountry**: Oyuncu kimlik ve sınıflandırma bilgileri.
- **Rating / TopRating**: Oyuncunun anlık ve ulaştığı en yüksek rating değerleri.
- **TotalDrop**: Toplam yatırılan para.
  - Formül: `(LG Total Drop) + (Slot Drop)`
  - Açıklama:
    - **LG Total Drop**: Masalarda yapılan toplam drop (cash + plaque).
    - **Slot Drop**: Slot tarafındaki toplam drop.
- **TotalResult**: Toplam oyun sonucu.
  - Formül: `(LG Total Result) + (Slot Result)`
  - Açıklama:
    - **LG Total Result**: LG tarafındaki toplam sonuç (oyun içi kazanç/kayıp).
    - **Slot Result**: Slot tarafındaki toplam kazanç/kayıp.
- **AvgDrop**: Ziyaret başına ortalama drop.
  - Formül: `TotalDrop / SlotPlayDays`
- **AvgResult**: Ziyaret başına ortalama sonuç.
  - Formül: `TotalResult / SlotPlayDays`
  - Not: 0'a bölme hatasını engellemek için `SlotPlayDays` değeri yoksa 1 alınır.
- **TotalLgResult**: LG tarafındaki toplam sonuç.
- **TotalSlotResult**: Slot tarafındaki toplam sonuç.
- **LgPlayDays**: LG oynanan gün sayısı.
- **SlotPlayDays**: Slot oynanan gün sayısı.
- **FirstVisitDate / LastVisitDate**: İlgili aralıktaki ilk/son ziyaret tarihleri.

---

## Girdi

- **StartDate / EndDate**: Oyun verilerinin toplandığı tarih aralığı.
- **BalanceCurrencyId**: Tutarların çevirildiği para birimi.
Örnek istek modeli:

```json
{
  "startDate": "2025-01-01",
  "endDate": "2025-01-31",
  "balanceCurrencyId": 1
}
```

---

## Çıktı

- Her kayıt bir oyuncunun özet verilerini içerir. Çıktı, `ReportFilteredOutput` listesi olarak döner.

Örnek cevap şeması:

```json
[
  {
    "playerId": 1,
    "playerName": "Ridotto Admin",
    "playerCategory": "Local",
    "playerClass": "A",
    "playerCountry": "Türkiye",
    "rating": "A",
    "topRating": "A+",
    "totalDrop": 10000.0,
    "totalResult": -750.0,
    "avgDrop": 500.0,
    "avgResult": -37.5,
    "totalLgResult": -250.0,
    "totalSlotResult": -500.0,
    "lgPlayDays": 4,
    "slotPlayDays": 20,
    "firstVisitDate": "2025-01-03",
    "lastVisitDate": "2025-01-29"
  }
]
```

---

## Notlar

- `AvgDrop` ve `AvgResult` hesaplarında 0'a bölmeye karşı koruma vardır; `SlotPlayDays` 0 ise 1 kabul edilir.
- Döviz çevrimleri, `BalanceCurrencyId` ye göre yapılmıştır.
- LG ve Slot metrikleri birleştirilirken tarih filtreleri `StartDate`–`EndDate` aralığına sıkı şekilde uygulanır.
