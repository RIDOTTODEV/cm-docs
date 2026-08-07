---
title: "Check-In"
layout: single
permalink: /registrationapp/check-in/
---

Bu ekran Registration App uygulamasının ilk sayfasıdır. Bu sayfadan her gelen misafir için bir check in oluşturulur ve geçmişe dönük olarak tüm misafirlerin check in kayıtları listelenir.

## Check-In Alan Açıklamaları

- **Id**: Tutulan kayıdın numarası (sistem tarafından atanan benzersiz numara).
- **F.Reg.Date**: Misafirin ilk giriş yaptığı tarih (Check in yapıldığında otomatik olarak girilir).
- **Name**:Misafir Adı (Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **Surname**:Misafir Soyadı (Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **Gender**:Misafir Cinsiyet (Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **BirthDate**:Misafir Doğum Tarihi (Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **Document Type**: Misafirin Casino oyuncu kartını çıkartırken kullandığı Resmi evrakların bilgisi(Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **National Id No**: Misafirin resmi evrağı üzerindeki benzersiz kimlik numarası(Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **Nation**: Misafirin resmi evrağının üzerinde bulunan ve hangi millete bağlı olduğunu gösteren bilgi(Misafirlerin kart çıkartma işlemi sırasında kaydedilen kimlik bilgileri üzerinden Casino oyuncu kartlarına işlenir ve o kartlar üzerinden bilgiler getirilir).
- **Time In**: Misafirin giriş yaptığı tarih ve saat bilgisi(Check In işlemi sırasında otomatik olarak doldurulur).
- **Check In Type**: Check In yapan kişinin misafir olarak mı yoksa staff olarak mı check in yaptığını tutar(Check In işlemi sırasında seçilir).
- **Status**: Giriş yapan misafirleri gruplamak için kullanılan etiketler(Check In işlemi sırasında seçilir).
- **Address**: Misafirin adres bilgisi

## Genel Kullanım

Uygulama açıldığında karşınıza üstte iki sekme bulunan bir ekran gelir. Sistem varsayılan olarak Check In sekmesiyle başlar. Bu sekme üzerinden yeni gelen her misafir için check in oluşturabilir, ayrıca geçmişe dönük check in kayıtlarını görüntüleyebilirsiniz.

![StickyTopNavbar]({{ '/assets/images/registrationapp/StickyNavbar.png' | relative_url }})

Check In sekmesinin araçlar kısmı bize 2 adet tarih ayarlama kutusu sunar bunlardan soldaki kutu başlangıç sağdaki ise bitiş tarihini temsil etmektedir bu kutulara tarih kısıtlarımızı girdikten sonra tarih kutularının yanında bulunan search butonuna basarak belirlediğimiz tarih aralığındaki kayıtları listeleyebiliriz.

![ToolsMenuDateInfo]({{ '/assets/images/registrationapp/ToolsMenuDateInfo.png' | relative_url }})

Bunun yanı sıra tarih kutularının yan tarafında bulunan arama kutusu üzerinden de tablo içerisindeki bilgilere göre kayıt araması yapılabilir ve eşleşen tüm kayıtlar kullanıcıya sunulur.

![ToolsMenuSearchInfo]({{ '/assets/images/registrationapp/ToolsMenuSearchInfo.png' | relative_url }})

Arama kısımlarının yanında bulunan PDF ve Excel butonları üzerinden rapor çıktısı alanabilir formatlar buton ismi üzerinde belirtildiği gibi hazırlanır ve indirmeye hazır bir şekilde kullanıcıya sunulur.

![ToolsMenuReportInfo]({{ '/assets/images/registrationapp/ToolsMenuReportInfo.png' | relative_url }})

Rapor çıktılarının yanında bulunan New Check In butonu ile gelen misafirlere yeni Check In oluşturulabilir.

![ToolsMenuCheckInInfo]({{ '/assets/images/registrationapp/ToolsMenuCheckInInfo.png' | relative_url }})

Check In kayıtları işlemler sekmesinin hemen altında bulunur ve kullanıcıya tablo formatında aldıkları statuslara göre renklendirilmiş bir şekilde sunulur.

![RecordsTable]({{ '/assets/images/registrationapp/RecordsTable.png' | relative_url }})

Tablonun altında yer alan Total Records alanı, listelenen toplam kayıt sayısını gösterir.

![TotalRecordCount]({{ '/assets/images/registrationapp/TotalRecordCount.png' | relative_url }})

## Check-In oluşturma

New Check-In butonuna tıklandıktan sonra önümüze küçük bir menü açılır bu menu üzerinden Check-In kaydı yapılabilir.

Önümüze açılan menü bize 2 seçenek sunar staff veya guest biz varsayılan olarak işlemlerimizi Guest (Misafir) üzerinden gerçekleştiririz.

![CheckInRadioButtons]({{ '/assets/images/registrationapp/CheckInRadioButtons.png' | relative_url }})

Hemen altında, misafir kaydının nasıl yapılacağını belirlediğimiz iki buton bulunur. Soldaki Scan Document butonu seçilirse, check in işlemi misafirin resmi evrakları üzerinden gerçekleştirilir. Sağdaki Player Card Scan butonu seçilirse, check in işlemi Card Reader'a takılı olan casino oyuncu kartı üzerinden gerçekleştirilir.

![ScanTypes]({{ '/assets/images/registrationapp/ScanTypes.png' | relative_url }})

Player Card Scan veya Document Scan butonuna basıldıktan sonra önümüze misafirin bilgileri gelir misafir bilgilerinin alt kısmında ise status etiketlerinin belirlenme kısmı vardır buradan belirlediğimiz etikete göre misafirler gruplanır.

![PlayerStatus]({{ '/assets/images/registrationapp/PlayerStatus.png' | relative_url }})
