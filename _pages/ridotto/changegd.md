---
title: "Ridotto Gün Değişimi"
parent: "Ridotto"
layout: single
nav_order: 3
permalink: /ridotto/changegd/
---

<!-- ## Genel Tanım
Casinolarda **oyun günü**, saat 00:00 – 23:59:59 aralığından farklı olarak, keyfi seçilmiş bir saatten başlayıp ertesi gün aynı saate kadar olan süredir.  
Örneğin: `20 Ağustos 03:55 – 21 Ağustos 05:13` arası tek bir oyun günü kabul edilir ve raporlarda bu aralık **20 Ağustos** olarak adlandırılır.  

Sistemde raporlama ve hesaplama yapılırken seçilen tarih, bu oyun günü karşılıklarına göre hesaplanır. -->

# Casino Gaming Date Yönetimi

## 1. Roller

- **Admin / Cashdesk Supervisor** → Gaming Date oluşturur, kasa gününü değiştirir.
- **Slot Inspector** → Slot makinelerinin gün değişimi ve sayımlarını yapar.
- **Table Inspector** → Masalardaki çip float sayımlarını yapar.
- **Cashier** → Kasa balansı, çip/cash/plaque hareketlerini yönetir.

---

## 2. Ana Akış

### 2.1. Yeni Gaming Date Oluşturma

- Ridotto üzerinde `Gaming Date` menüsünden yeni gün oluşturulur.
- Bu gün, makinelerin ve masaların geçirileceği referans gündür.

{% include figure popup=true image_path="/assets/images/gamingdate-create.png" alt="Gaming Dates" caption="Gaming Dates" %}

### 2.2. Slot Operasyonları

- Slot makinelerinin bill acceptor box'ları değişimi yapılır.
- `Slots` menüsünden makineler **tek tek** veya **toplu** olarak yeni güne geçirilir.
- Geçirilen makinede yapılan tüm kredi açma/silme ve oyun kayıtları artık **yeni güne** işlenir.
- GamingDate menüsünden önceki günün satırının açılır menüsünden `Slot Count Form` açılarak makinelerin bill acceptor box sayımları girilir.
  - **Beklenen = Sayım** → değerler **yeşil** görünür.
  - **Fark var** → değerler **turuncu** görünür.

### 2.3. Masa Operasyonları

- Inspector’lar kendi panelinden masalardaki çip floatlarını sayar ve sisteme girer.

{% include figure popup=true image_path="/assets/images/inspector-chip-count.png" alt="Inspector Chip Count" caption="Inspector Count" %}

- `Table Operations → Count` ekranında:
  - Masanın cash ve plaque box değerleri girilir. Ayrıca inspectorların çip sayımları burada görünür.
  - Sistem ile sayım arasındaki farklar gösterilir (**yeşil/turuncu**).

{% include figure popup=true image_path="/assets/images/table-count.png" alt="Table Count" caption="Table Count" %}

- Sayım tamamlandıktan sonra masalar seçilerek **float resetleme** yapılır:
  - Fazla çip → kasaya aktarılır.
  - Eksik çip → kasadan tamamlanır.
  - İşlem seçilen transaction code ile kasa kayıtlarına ve balansına yansır.

### 2.4. Masa Gün Değişimi

- Masalar tek tek veya topluca yeni güne geçirilir.
- Masaların plaque ve cash sayımları kasa işlemlerine otomatik yansır.
- Gün değişen masadaki işlemler artık **yeni güne** kaydedilir.

### 2.5. Kasa Gün Değişimi

- Kasa, son güne geçirilmedikçe üst bar’da **Change Gaming Date** butonu görünür.
- Gün değişimi yapıldığında:
  - Üst bar **yeşil** olur.
  - `2/2` → Tüm kasalar güncel.
  - `8/8` → Tüm masalar güncel.
- Eksik varsa değerler **kırmızı** görünmeye devam eder.

---

## 3. Tamamlanma Kriteri

- **Tüm masalar** + **kasa** son güne geçirildiğinde oyun günü değişimi tamamlanmış sayılır.
- Bu andan itibaren tüm raporlar ve hesaplamalar yeni gün üzerinden yapılır.

---

## 4. Görsel Durum İpuçları

- **Yeşil** → İşlem/fark yok, güncel.
- **Turuncu** → Sayım farkı var.
- **Kırmızı** → Henüz yeni güne geçirilmemiş kasa/masa.
