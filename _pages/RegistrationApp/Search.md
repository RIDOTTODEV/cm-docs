---
title: "Search"
layout: single
permalink: /registrationapp/search/
---

Bu sayfa RegistrationApp uygulamasının ikinci sekmesidir.
Bu sayfa üzerinden yeni gelen misafirin casinoya kayıtları yapılabilir. Casino oyuncu kartları çıkartılabilir, bilgileri güncellenebilir, kart basılabilir ve misafirin sahip olduğu tüm kartlar izlenebilir.
Müşterilere birden fazla resmi evrak bilgisi yüklenebilir(Ehliyet, Kimlik, Pasaport).
Sistem üzerinde misafir adı veya misafir assist benzersiz id ile misafirler aranabilir.
Casino misafirlerinin yaklayaşan doğum günleri izlenebilir.

## Search Upcoming BirthDays Alan açıklamaları

- **Full Name**: Misafir Adı Soyadı.
- **Birth Day**: Misafir Doğum Tarihi(Gün/Ay).
- **Assist Id**: Misafirin Assist programına kaydedilmiş benzersiz numarası.
- **Player Id**: Misafirin Riddotto üzerindeki benzersiz numarası.

Sayfayı ilk açtığımızda bizi yaklaşan doğum günleri, arama çubuğu ve bunun hemen yanında anasayfa ve oyuncu kayıt butonu bizi karşılar.

Hemen altında ise geçmiş aramalarımıza hızlıca ulaşabilmemiz için son aramalarımız listelenir.

![SearchHomePage]({{ '/assets/images/registrationapp/SearchHomePage.png' | relative_url }})

Sayfada bir misafirin araması yapıldığı zaman veya bir kart takılarak detay sayfasına girildiği zaman bizi misafir adı,soyadı,assistId,riddottoId(PlayerId) ve fotoğrafı bize sunulur. Hemen alt kısmında ise Kart çıkartma, yeni kart tanımlama ve misafir bilgilerini düzenlediğimiz 3 adet buton bulunur.

Bunun altında, misafire ait tüm kartları görüntüleyebileceğimiz bir tablo bulunur. Bu tabloda şu bilgiler yer alır:

- **CardId** — Tanımlanan kartın benzersiz numarası
- **CreationTime** — Kartın misafir için oluşturulduğu tarih ve saat
- **Action** — Kartı deaktif edebileceğimiz aksiyon butonu

![DetailScreenInfo]({{ '/assets/images/registrationapp/DetailScreenInfo.png' | relative_url }})

Tablonun sağ tarafında ise misafirin resmi evraklarının yüklenebileceği bir kısım bulunur.Dosya Ekle butonuna tıklayarak üst kısımda bulunan kutuya dosyanın adı girilmelidir(Dosya adı zorunlu alandır) alt kısımda bulunan File kutusuna ise çalışma ortamımızda bulunan ve sadece PDF, JPG ve PNG formatında olan evraklar yüklenebilir(Dosya alanının doldurulması zorunludur).

Oyuncu Kayıt Butonu içerisinde isim, soyisim, country, birthday, gender, fotoğraf gibi alanlar zorunludur. Eğer kimlik kartı vb bir evrak kullanarak kayıt yaparsak otomatik olarak bizim alanlarımız doldurulur. Kamerayı açmak için ise Player Profile Photo kısmındaki video işaretine basılması ardından fotoğrafı çekmek için ise kamera işaretine basılması gerekmektedir.

⚠️Kimlik Kartı ile oyuncu kaydı yapılırken ilk olarak kimliğin arka tarafı okutulmalıdır⚠️

![AddingPlayer]({{ '/assets/images/registrationapp/AddingPlayer.png' | relative_url }})
