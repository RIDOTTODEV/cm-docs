---
title: "Order Page"
layout : single 
permalink : /pashaposkiosk/orderspage/
---

## Orders Sayfası ve Bekleyen Siparişler 

Orders butonuna tıklandığında, teslim edilmesi beklenen siparişlerin listelendiği sayfası açılır.

Bu sayfada, her bekleyen sipariş için sipariş bilgilerini içeren bir ticket bulunmaktadır. Bu ticket içerisinde siparişin hangi garson tarafından verildiği, siparişin gönderileceği slot makinesinin numarası veya Live Game masasının adı, siparişin oluşturulduğu saat, dakika ve saniye bilgileri ile sipariş içerisindeki ürünlerin listesi yer alır.

Ticket'ın en altında bulunan New Ticket butonu, sipariş teslim edildiğinde kullanılır. Butona tıklandığında ilgili sipariş ticket'ı bekleyen siparişler listesinden kaldırılır.

![undeliveredorders]({{ '/assets/images/pashaposkiosk/undeliveredorders.png' | relative_url }})

### Clear All Ticket Butonu

Sayfanın sağ üst köşesinde bulunan Clear All Ticket butonu, teslim edilmiş olan tüm siparişleri tek seferde listeden kaldırmak için kullanılır. Bu sayede siparişleri tek tek kapatmak yerine, tüm siparişler teslim edildiyse tek bir butonla tamamı kapatılabilir.

### Creta New Order Butonu

Create New Order butonu, yeni bir sipariş oluşturma ekranına geçiş yapmak için kullanılır. Bu butona tıklandığında kullanıcı, yeni sipariş oluşturma bölümüne yönlendirilir.


![ClearandCreate]({{ '/assets/images/pashaposkiosk/ClearandCreate.png' | relative_url }})

### Search Bölümü 

Search kutusu, bekleyen siparişler arasında hızlı bir şekilde arama yapılmasını sağlar. Arama yapabilmek için sadece garson adı veya masa numarası girilmelidir.


![ticketsearch]({{ '/assets/images/pashaposkiosk/ticketsearch.png' | relative_url }})

### Order History 

Order History bölümü, daha önce oluşturulmuş ve teslim edilmiş siparişlerin listelendiği bölümdür. Bu sayfanın sağ üst kısmında bulunan Search özelliği ile geçmiş siparişler arasında arama yapılabilir. Ayrıca tam ekran görünümüne geçilebilir ve sipariş listesi güncellenebilir.

Siparişlerin yanında bulunan Replay butonu, teslim edilmiş ve Order History bölümüne aktarılmış olan siparişlerin statüsünü değiştirerek tekrardan orders listesine almamızı sağlar. Bu sayede yanlışlıkla teslim edilmiş olarak işaretlenen veya henüz teslim edilmemiş bir sipariş, tekrar teslim bekleyen siparişler arasına alınabilir.

Sayfanın alt kısmında ise listede bulunan toplam sipariş sayısı görüntülenir. Ayrıca siparişlerin sayfada kaç adet gösterileceği belirlenerek listeleme düzeni ayarlanabilir.

![OrderHistory]({{ '/assets/images/pashaposkiosk/OrderHistory.png' | relative_url }})





















