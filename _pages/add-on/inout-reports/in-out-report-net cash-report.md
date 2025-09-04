---
title: "In-out Net Cash Summary Report"
parent: "In/Out Reports"
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
sidebar:
  nav: "inout-reports"
---

## In-out Net Cash Summary Report

Belirtilen tarih aralığında oyuncuları kategori (PlayerCategory) bazında gruplayarak; LG sonucu, Slot sonucu, harcama (expense), doküman ve net nakit (Net Cash) özetlerini üretir.

---

## Özellikler ve Açıklamalar

- **PlayerCategory**: Grup anahtarı. Oyuncunun kategorisi (ör. Local/Foreign vb.).
- **PlayerCount**: İlgili kategorideki ziyaret sayıları toplamı.
- **TotalLgResult**: LG tarafındaki toplam sonuç.
- **TotalSlotResult**: Slot tarafındaki toplam sonuç.
- **TotalResult**: Toplam oyun sonucu.
    - Formül: `TotalLgResult + TotalSlotResult`
- **GamingExpense**: Toplam oyun harcaması(Disc+com vb. Transaction code daki gamingexpense işaretli olanların toplamı)
- **Documents**: Oyuncularla ilişkili belge toplamları (çek+senet vb. Transaction code daki documents işaretli olanların toplamı)
- **GamingLoss**: Harcama dahil oyun kaybı göstergesi.
    - Formül: `TotalLgResult + TotalSlotResult + GamingExpense`
- **NetCash**: Net nakit.
    - Formül: `TotalResult - (GamingExpense + Documents)`
    - Açıklama: Oyun sonuçlarından harcama ve belgeler düşülür.

---
