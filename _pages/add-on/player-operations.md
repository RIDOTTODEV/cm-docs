---
title: "Player Operations"
parent: "Add-on"
layout: single
nav_order: 2
permalink: /add-on/player-operations/
toc: true
toc_sticky: true
---

# Player Operations

## Overview
**Player Operations** modülü, kasadaki işlemleri oyuncular bazında yönetmek ve takip etmek için kullanılır. Bu ekran üzerinden oyuncuların **cashless hesaplarına yatırma/çekme işlemleri**, geçmiş işlemler, arama ve son aramalar gibi bilgiler görüntülenebilir.

---

## 1. Player Operations Ana Ekranı

### 1.1 Search Players
- **Arama Çubuğu**: Oyuncuları **isim, soyisim, e-posta veya telefon numarası** ile aramayı sağlar.
- **Last Searches**: Son aranan oyuncular listelenir.
- Her oyuncunun yanında hızlı erişim için bir **sağ ok butonu** bulunur.

### 1.2 Cash Desk Summary
Kasa hareketlerinin özetini iki bölümde gösterir:

1. **Hesap Türüne Göre Özet**
   - Account Type (Örn: Cashable)
   - Transaction Type (Deposit, Withdrawal vb.)
   - EUR ve TL bazında toplam tutar

2. **Kasaya Göre Özet**
   - Cashdesk adı (Örn: Main Cashdesk)
   - Account Type
   - Transaction Type
   - EUR ve TL tutarları

---

## 2. Player Detail Ekranı

### 2.1 Oyuncu Bilgileri
- **Fotoğraf** (Varsayılan: No Photo)
- Oyuncu Adı ve ID
- Default Currency
- Blacklist Durumu
- Player Class ve Discount bilgisi (Oyuncuya özel Discount oranı belirlenmiş ise getirir)
- **Son Görülme Tarihi**

#### Durum Göstergeleri
- **Is Active**: Oyuncunun aktif olup olmadığını gösterir.
- **Discount**: Oyuncunun discount alabilir olup olmadığı durumu.

### 2.2 Ek Bilgiler
- **Friends List**: Oyuncunun arkadaş listesi
- **General Notes**: Genel notlar
- **PR Notes**: Halkla ilişkiler notları

---

## 2.3 İşlem Butonları
- **Cage Transaction**
  Oyuncu için cashless ve ya çip karşılığı olmayan işlerin girilebileceği formu açar
- **In Out Transactions**
  Oyuncu için tarih aralığına göre rapor sunar
- **In Out Selected Name Report**  
  Oyuncunun tarih aralığına göre:
  - Masa ve slot oyun geçmişi & sonuçları
  - Yatırım ve çekim toplamları
  - Expense & fee giderleri
  - Otel konaklama, uçak bileti vb. harcamalar

- **Today**: Bugünkü işlemleri filtreler

---

## 3. Cashless ve Chip İşlemleri

### 3.1 Tablar
- **Cashless**: Slot makineleri için elektronik hesap işlemleri
- **Chip**: Masa oyunları için çip işlemleri

### 3.2 Hesaplar
Her para birimi için ayrı hesap kartı:
- Gün içinde Toplam Giriş (Total In)
- Gün içinde Toplam Çıkış (Total Out)
- **Deposit**: Para yatırma
- **Withdraw**: Para çekme
- **History**: İşlem geçmişi

### 3.3 İşlem Türleri
- Cash
- Credit
- Çek
- Banka Transferi
- ..

---

## 4. Cage Transactions
Oyuncunun kasa işlemleri:
- **Created At**: İşlem tarihi
- **Transaction Type**: Paid / Received
- **Trans Type**: Player için Transaction Tipi
- **Transaction Code**: Kasa için Transaction kodu
- **Amount**: İşlem tutarı (para birimi ile)
- **Station**: İşlemin yapıldığı kasa

Renk Kodları:
- **Kırmızı**: Paid (kasadan para çıkışı)
- **Yeşil**: Received (kasaya para girişi)

---

## Örnek Senaryo
1. Oyuncu aranır veya son aramalardan seçilir.
2. Oyuncu detay sayfasına girilir.
3. Cashless veya Chip sekmesinden işlem yapılır.
4. Gerekirse **In Out Selected Name Report** ile geçmiş raporu alınır.
