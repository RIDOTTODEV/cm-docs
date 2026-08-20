---
title : "Stock Management"
layout : single 
permalink : /pashapospanel/stockmanagement/
---

## Stock Managment 

Stock Management bölümü, casino içerisinde bulunan ürünlerin stok takibinin yapılmasını sağlayan paneldir. Bu bölüm üzerinden hangi üründen kaç adet bulunduğu takip edilebilir.

Stock In işlemi ile stoğa yeni ürünler eklenerek stok miktarı güncellenir. Stock Out işlemi ise zayi olan veya kaybolan ürünlerin stoktan düşülmesini sağlamak için kullanılır. Böylece ürünlerin mevcut stok durumu düzenli olarak takip edilebilir.

### Stock Overview

Panelin ilk sayfasında Stock Overview bölümü bulunmaktadır. Bu bölümde, casino içerisindeki ürünlerin stok durumlarının görüntülendiği uzun bir ürün tablosu yer alır.

Tabloda ürünlere ait çeşitli bilgiler bulunmaktadır. Bunlar arasında Product Name, ürünün bağlı olduğu Tag, Shop, Total ve Movement gibi alanlar yer alır. Total alanı, ilgili ürünün casino genelinde toplam ne kadar stokta bulunduğunu gösterir. Bunun yanında, ürünün hangi bar veya depoda ne kadar bulunduğu da görüntülenebilir. Tablonun en sağında ise stok hareketlerinin takip edilebildiği Movement ve Detail bölümleri bulunmaktadır.


![StockOverview]({{ '/assets/images/pashapospanel/StockOverview.png' | relative_url }})

Tablonun üst kısmında ürünleri daha kolay bulabilmek için çeşitli filtreleme seçenekleri yer almaktadır. Product Tag, Product Category ve Product Name gibi filtreler kullanılarak istenilen ürünlere daha hızlı ulaşılabilir.

Tablonun yanında ise Stock Action bölümü bulunmaktadır. Bu bölüm üzerinden Stock Out, Stock In, Transfer, Sayım ve Sayım Geçmişi gibi stok işlemleri gerçekleştirilebilir.

![filterandaction]({{ '/assets/images/pashapospanel/filterandaction.png' | relative_url }})


### Stock In

Stok miktarını artırmak, yani yeni bir ürün alımı gerçekleştirmek için Stock In işlemi kullanılır. Stock In seçeneğine tıklandığında öncelikle Select Template ekranı açılır. Bu ekranda daha önce kaydedilmiş stok alım şablonları listelenir. Kullanıcı, daha önce oluşturulmuş bir şablonu seçerek işlemi hızlı bir şekilde gerçekleştirebilir.

Yeni bir stok alımı yapılacak ve kayıtlı şablonlardan biri kullanılmayacaksa, ekranın alt kısmında bulunan Stock In From Scratch seçeneği kullanılır. Bu seçenek, stok alım işlemini sıfırdan oluşturmayı sağlar.

![SaveTemplate]({{ '/assets/images/pashapospanel/SaveTemplate.png' | relative_url }})


Stock In ekranında sol tarafta ürünlerin listelendiği bir tablo bulunmaktadır. Bu tabloda Product Name ve Current Stock bilgileri görüntülenirken, Piece alanına satın alınan ürün miktarı girilir. İstenirse ilgili ürün için Note alanına açıklama da eklenebilir.

Ekranın sağ tarafındaki Save Stock Entries bölümünde ise stok alımının yapılacağı Location seçilir. Ardından alımın nedeni Reason alanından belirlenir. Gerekli görülmesi durumunda Note alanına ek bir açıklama girilebilir.

Tüm bilgiler girildikten sonra Save butonuna basılarak stok alımı kaydedilir. Kaydedilen miktar, seçilen lokasyona eklenir ve Stock Overview bölümündeki mevcut stok miktarı buna göre güncellenir. Böylece satın alınan ürünler stoklara eklenmiş olur.

![StockInLogin]({{ '/assets/images/pashapospanel/StockInLogin.png' | relative_url }})

### Stock Out 

Stock Out bölümünde, Stock In işlemine benzer bir ekran bulunmaktadır. Ancak bu işlemde ürünler stoğa eklenmek yerine mevcut stoktan düşülür.

Ekranın sol tarafında ürünlerin listelendiği tablo yer alır. Stock Out işlemi yapılacak ürünler için ilgili miktarlar Piece alanına girilir. Böylece hangi üründen kaç adet stoktan düşüleceği belirlenir.

Ekranın sağ tarafında ise Save Stock Entries bölümü bulunmaktadır. Burada, ürünlerin hangi Location üzerinden stoktan düşüleceği seçilir. Reason alanında ise stoktan düşme nedeni olarak iki seçenek sunulur: Zayi ve Kayıp. Yapılan işleme uygun neden seçildikten sonra istenirse Note alanına ek bir açıklama girilebilir.

Gerekli bilgiler girildikten sonra Save butonuna basılarak işlem tamamlanır. Kaydedilen miktarlar ilgili lokasyonun stokundan düşülür ve Stock Overview bölümündeki stok miktarları buna göre güncellenir.

![StockOutLogin]({{ '/assets/images/pashapospanel/StockOutLogin.png' | relative_url }})


### Transfer 

Transfer bölümü, bir ürünün bir bar veya depodan başka bir bar ya da depoya aktarılması gerektiğinde kullanılır. Bu işlem sayesinde mevcut stok, bir lokasyondan başka bir lokasyona taşınabilir.

Transfer ekranının sol tarafında ürünlerin listelendiği bir tablo bulunmaktadır. Transfer edilmek istenen ürün için ilgili alana kaç adet ürünün aktarılacağı girilir. Ardından ekranın ilgili bölümünden ürünün hangi bar veya depodan alınacağı ve hangi bar veya depoya aktarılacağı seçilir.

Gerekli bilgiler girildikten sonra Save butonuna basılarak transfer işlemi tamamlanır. Transfer işlemi genel stok miktarını değiştirmez; yalnızca ürünün bulunduğu lokasyon değişir. Bu nedenle Shop Total değerinde herhangi bir azalma veya artış olmaz, yalnızca ilgili bar veya depoların stok miktarları arasında değişiklik gerçekleşir.

![TransferLogin]({{ '/assets/images/pashapospanel/TransferLogin.png' | relative_url }})

### Count 

Sayım bölümü, mevcut stokların fiziksel olarak kontrol edilmesi ve sistemde kayıtlı olan stok miktarlarıyla karşılaştırılması için kullanılır. Sayım sırasında elde bulunan gerçek ürün miktarları ilgili alanlara girilir.

Sistem, girilen miktarları otomatik olarak mevcut stok miktarlarıyla karşılaştırır. Girilen miktar ile sistemde kayıtlı olan stok miktarı arasında bir fark olması durumunda, miktar fazla veya eksik olsa dahi ilgili ürün için kırmızı bir uyarı gösterilir. Böylece stok miktarındaki farklılıklar kolayca tespit edilebilir.

Ayrıca her ürün için Note alanına açıklama eklenebilir. Sayım işlemi tamamlandıktan sonra Save butonuna basılarak kayıt oluşturulur. Eğer sayım ile stok arasında fark varsa save ederken sorar stock ile sayım arasında fark var yine de stock a uygulansın mı diye evet derseniz yeni sayım daki ürünler stock a işlenir. Kaydedilen sayım işlemleri daha sonra Count History bölümünden görüntülenebilir.


![StockSayımEkranı]({{ '/assets/images/pashapospanel/StockSayımEkranı.png' | relative_url }})

### Count History 

Sayım işlemi tamamlanıp Save butonuna tıklandıktan sonra, yapılan sayım Count History bölümüne kaydedilir. Bu sayfada, daha önce gerçekleştirilen sayımların listelendiği bir tablo bulunmaktadır. Her sayım, tabloda ayrı bir satır olarak kayıt altına alınır.


![OrderHistory]({{ '/assets/images/pashapospanel/OrderHistory.png' | relative_url }})

Her satırın en sağında bulunan Detail butonuna tıklandığında, ilgili sayımın detaylarını gösteren yeni bir tablo açılır. Bu tabloda ürün adları, sayım sonucunda tespit edilen miktar ve sayım öncesinde stokta bulunan beklenen miktar bilgileri yer alır. Bu sayede sayım sonucunda elde edilen miktar ile sistemde kayıtlı olan stok miktarı kolayca karşılaştırılabilir.

![DetayOrderHistory]({{ '/assets/images/pashapospanel/DetayOrderHistory.png' | relative_url }})

### Movements

Stock Management bölümünün başlangıcında yer alan Stock Overview tablosunda, ürünlerin bulunduğu lokasyonları gösteren sütunun hemen yanında Movement bölümü bulunmaktadır. Bu bölüm, ürünlerin stok hareketlerinin detaylı olarak takip edilmesini sağlar. Ürüne yapılan Stock In, Stock Out ve Transfer işlemlerinin tamamı bu bölüm üzerinden görüntülenebilir.

Örneğin, EVE 120 S isimli sigara üzerinden ilerlediğimizde, bu ürüne ait tüm stok hareketlerini görebiliriz. Hareket geçmişinde 1 adet Stock Entry, 1 adet Stock Out ve 4 adet Transfer işlemi bulunmaktadır.

İlk olarak Stock In işlemiyle üründen 1000 adet stoğa giriş yapılmıştır. Daha sonra Stock Out işlemi ile 20 adet ürün zayi olarak stoktan düşülmüştür. Ardından ürünün farklı barlara aktarılması için 2 transfer işlemi gerçekleştirilmiş ve her bir transferde 200 adet ürün ilgili barlara gönderilmiştir.

Bu şekilde Movement bölümü üzerinden bir ürünün stoğa girişinden, stoktan çıkışına ve farklı lokasyonlara transfer edilmesine kadar gerçekleşen tüm stok hareketleri detaylı olarak takip edilebilir.

![Movements]({{ '/assets/images/pashapospanel/Movements.png' | relative_url }})




 