---
title: "Reports"
layout: single 
permalink: /pashapospanel/Reports/
---

## Report Sayfası 

### Product Orders
Bu bölümde, tüm menülerde bulunan ürünlerin listelendiği bir tablo bulunmaktadır. Tabloda Product Name, Portion Name ve Order Count bilgileri yer alır. Order Count, ilgili üründen toplam kaç adet sipariş oluşturulduğunu gösterir.

Tablonun üst panelinde ise çeşitli işlem ve filtreleme seçenekleri bulunmaktadır. Search özelliği ile ürünler arasında arama yapılabilir. Today seçeneği üzerinden hangi tarihe kadar olan verilerin görüntüleneceği belirlenebilir. Replay butonu tabloyu yenilemek, Full Screen butonu tabloyu tam ekran görüntülemek ve Download/Export butonu ise tablo verilerini dışa aktarmak için kullanılır.

![ProductTable]({{ '/assets/images/pashapospanel/ProductTable.png' | relative_url }})

### Player Order By Tag 

Player Order by Tag tablosunda Player Name, Player ID, Assist ID, Player Tag Name, Total Order Count ve Quantity kolonları bulunmaktadır.

Bu tablo sayesinde, belirli bir Player ID'ye sahip oyuncunun hangi ürün kategorisinden kaç kez sipariş verdiği ve toplam kaç adet ürün aldığı görüntülenebilir. Bu bilgiler, oyuncuların sipariş alışkanlıklarının takip edilmesi ve raporlama süreçlerinin oluşturulması açısından faydalıdır.

Yine her tabloda olduğu gibi bu tabloda da tam ekran yapabiir ve export edebiliriz. Ayrıca tarih bölümünden en son hangi aralıkta ki verileri istiyorsak seçebiliriz ve search ksımından daha detaylı arama yapılabilir. 

![PlayerOrderByTagTable]({{ '/assets/images/pashapospanel/PlayerOrderByTagTable.png' | relative_url }})

### Order By Category 

Bu tablo, menüde bulunan ürün kategorilerini ayrı ayrı listeleyerek her kategoriden kaç sipariş oluşturulduğunu ve toplam kaç adet ürün gönderildiğini gösterir. Bu sayede hangi kategoriden kaç adet sipariş verildiği ve toplamda kaç ürün gönderildiği kolayca takip edilebilir.

Ayrıca bu tablo da da hepsinde olduğu gibi search kısmı bulunur. Order tag ve order category seçerek arama yapabilir yada daha detaylı arama için search yerinden direkt kategory nin isminş yazarak arama yapılabilir.

![OrderByCategory]({{ '/assets/images/pashapospanel/OrderByCategory.png' | relative_url }})   

- **Action Bölümü :** Bu bölümde Order Detail ve JSON Detail olmak üzere iki farklı seçenek bulunmaktadır. Her satırın yanında büyüteç ve code brackets (</>) simgeleri yer alır. Büyüteç simgesi, ilgili siparişin Order Detail bilgilerini görüntülemek için kullanılırken, code brackets (</>) simgesi siparişe ait JSON verilerini görüntülemek için kullanılır.

- Order Detail : Order Detail: Her satırdaki ürün kategorisine ait siparişlerin detaylarını gösteren tablodur. Bu tabloda, ilgili kategoride hangi üründen kaç adet sipariş verildiği ve toplam miktarı görüntülenir. Her satır için, yalnızca o satıra ait bağımsız bir Order Detail tablosu açılır.

![OrderDetail]({{ '/assets/images/pashapospanel/OrderDetail.png' | relative_url }}) 

- Json Kodları : Bu bölümde, siparişe ait JSON verileri görüntülenmektedir. JSON verileri sayesinde siparişlerin ID bilgisi, sipariş miktarı, ürün kategorisi ve diğer ilgili detaylarına daha ayrıntılı şekilde ulaşılabilir. Bu bölüm, sipariş verilerinin teknik olarak incelenmesini ve daha detaylı bilgi edinilmesini sağlar. 

![OrderByCategoryJson]({{ '/assets/images/pashapospanel/OrderByCategoryJson.png' | relative_url }}) 

### Cigarette Orders By Player 

Bu tablo, hangi oyuncunun kaç adet sigara siparişi verdiğini ve toplamda kaç adet sigara aldığını gösteren detaylı bir tablodur. Tablo, sigara siparişlerine özel olarak hazırlanmıştır.

Tablonun ilk sütunlarında Player Name ve Product Tag Name bilgileri yer alır. Product Tag Name alanı, bu tablonun yalnızca sigara siparişlerini içerdiğini belirtir. Ayrıca Order Count, oyuncunun kaç kez sigara siparişi verdiğini; Quantity ise toplam kaç adet sigara aldığını gösterir.

Ayrıca tabloda Player Name alanı boşsa, siparişin belirli bir oyuncuya değil, doğrudan bir slot makinesine verildiği anlamına gelir. Yani sipariş oluşturulurken bir oyuncu seçilmemiş, sipariş doğrudan slot makinesi için oluşturulmuştur.
Örneğin ilk satırda player name boş o zaman bu demek oluyor ki makineye girilmiş. 

![CigaretteOrderByPlayer]({{ '/assets/images/pashapospanel/CigaretteOrderByPlayer.png' | relative_url }})



















