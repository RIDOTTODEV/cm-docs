---
title: "Time In/Out Report"
parent: "Reports"
layout: single
nav_order: 2
permalink: /add-on/reports/time-in-out-report/
read_time: true
toc: true
toc_sticky: true
categories:
  - Report
tags:
  - Player
  - Report
---

## Time In/Out Report

Seçilen tarih aralığında oyuncu bazlı oturum (masa giriş/çıkış) kayıtlarını listeler.




- **PlayerId**: Oyuncunun id değeri.
- **PlayerFullName**: Oyuncunun ad ve soyadı.
- **Table**: Masanın adı.

- **InTime**: Oyuncunun masaya oturma zamanı.
- **OutTime**: Oyuncunun masadan kalkma zamanı. Çıkış yapılmadıysa `boş` olabilir.
- **PlayTime**: Oturum süresi dakika cinsinden. 

- **AvgBet**: Oturum boyunca eldeki kayıtların gösterdiği ortalama bahis tutarı . Para birimi, oturumun para birimidir.
- **CashDrop**: Oturum boyunca masaya yapılan nakit drop toplamı.
- **ChipDrop**: Oturum boyunca kasadan masaya yapılan chip/plaque drop toplamı .
- **Out**: Oyuncunun masadan kalkarkenki kasadan aldığı toplam (çıkış bakiyesi) .
- **Result**: `CashDrop + ChipDrop - Out` şeklindedir.

