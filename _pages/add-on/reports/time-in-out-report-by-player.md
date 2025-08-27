---
title: "Time In/Out Report By Player"
parent: "LG Reports"
layout: single
nav_order: 3
permalink: /lg/time-in-out-report-by-player/
read_time: true
toc: true
toc_sticky: true
categories:
  - Report
tags:
  - Player
  - Report
---

## Time In/Out Report By Player

Seçilen tarih aralığında oyuncu bazlı oturum (masa giriş/çıkış) kayıtlarını player bazlı toplu olarak hesaplar.


- **PlayerId**: Oyuncunun id değeri.
- **PlayerName**: Oyuncunun ad ve soyadı.
- **TotalPlayTime**: Oyuncunun tüm oturumlarının toplam süresi.

- **TotalAvgBet**: Oyuncunun tüm oturumlarındaki ortalama bahis tutarı. Ağırlıklı ortalama hesaplanır: `(AvgBet × HandCount) / TotalHandCount`
- **TotalCashDrop**: Oyuncunun tüm oturumlarındaki nakit drop toplamı.
- **TotalChipDrop**: Oyuncunun tüm oturumlarındaki plaque drop toplamı.
- **TotalOut**: Oyuncunun tüm oturumlarından kalkerken ki chip out toplamı
- **TotalResult**: Oyuncunun tüm oturumlarındaki sonuç toplamı 

- **TotalHandCount**: Oyuncunun tüm oturumlarındaki el sayısı toplamı 
- **Theoretical**: Teorik kazanç hesaplaması 
  - Formül:  `Oyun süresi × OrtalamaBahis × ElSayısı × HouseEdge`
