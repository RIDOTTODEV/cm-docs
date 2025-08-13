---
title: "Cage Operations"
parent: "Add-on"
layout: single
nav_order: 1
permalink: /add-on/cage-operations/
toc: true
toc_sticky: true
categories:
  - Add-on
tags:
  - Cage
---

# Cage Operations (Kasa İşlemleri) Sayfası

Bu sayfa, **Cage Operations** yani **Kasa İşlemleri** ekranıdır.  
Kullanıcıların kasa ve çip hareketlerini takip etmesini, günün işlemlerini görüntülemesini ve gerekli durumlarda düzenleme yapmasını sağlar.

---

## Genel Görünüm

Ekran iki ana bölümden oluşur:

- **Üst Menü Sekmeleri**:
  - **Account List**: Günün yapılan işlemlerinin listelendiği ana sekme.
  - **Cage Transactions**: Kasa ile ilgili tüm nakit işlemlerinin detaylı listesi.
  - **Chip Transactions**: Çip ile ilgili tüm hareketlerin listesi.
  - **Balance**: Güncel nakit bakiyesi.
  - **Chip Balance**: Güncel çip bakiyesi.

- **Sağ Üst Bakiye Bilgisi**:
  - **Cash**: Seçili kasadaki güncel nakit balansı.
  - **Chip**: Seçili kasadaki güncel çip balansı.

Bu bakiyeler, **üstte seçili olan kasa** üzerinden hesaplanır ve ekrana yansıtılır.  
Ayrıca yapılan tüm işlemler, **giriş yapan kullanıcı** yetkileri ve kullanıcı bilgileri ile ilişkilendirilir.

---

## Account List Sekmesi

Bu sekmede günün yapılan tüm işlemleri, **Transaction Code**’lara göre listelenir.  
Liste iki ana tabloya ayrılmıştır:

### 1. Cash Accounts (Nakit Hesaplar)
- **Account Name**: Hesap adı (ör. *Cash - Cash TL*, *Cash - Bank EUR*)
- **Currency**: Para birimi.
- **Transaction Code**: İşlem tipi (Cash, Bank, Bond vb.).
- **Total In**: Gün içindeki toplam giriş.
- **Total Out**: Gün içindeki toplam çıkış.
- **Result**: Net sonuç (giriş – çıkış).
- **Actions**: Geçmiş işlemleri görüntüleme butonu (*History*).

### 2. Chip Accounts (Çip Hesaplar)
- **Account Name**: Hesap adı (ör. *Chip - Cashdesk EUR*, *Chip - Credit Card EUR*).
- **Currency**: Para birimi.
- **Transaction Code**: İşlem tipi (Cashdesk, Credit Card, Discount vb.).
- **Total In**: Gün içindeki toplam giriş.
- **Total Out**: Gün içindeki toplam çıkış.
- **Result**: Net sonuç.
- **Actions**: Geçmiş işlemleri görüntüleme butonu.

---

## Özellikler
- Her iki tablo da **arama alanı** ile filtrelenebilir.
- Tüm rakamlar, **önceki gün kapanış + gün içi işlemler** formülüne göre hesaplanır:
  - **Kasa Balans Hesabı** = (Önceki gün kapanış) + (Bugünkü işlemler) - kasanın bakiyesi
  - **Chip Balans Hesabı** = (Önceki gün kapanış) + (Bugünkü chip işlemleri) - kasanın çip bakiyesi
- Sağ üstteki bakiyeler otomatik olarak güncellenir.
- **History** butonu ile ilgili hesabın geçmiş işlem detaylarına ulaşılır.

---

## Kullanım Senaryosu
Bu sayfa üzerinden:
1. Günün nakit ve çip hareketleri incelenir.
2. Bakiyeler kontrol edilir.
3. Hatalı veya eksik girişler düzeltilir.
4. Hesap geçmişleri incelenerek doğrulama yapılır.

---

**Not:** Görüntülenen tüm işlemler, yalnızca seçili kasa ve giriş yapan kullanıcıya göre filtrelenmiştir.  
