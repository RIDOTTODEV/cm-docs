---
title: "New Order"
layout: single 
permalink : /rubyposapp/neworder/
---

## New Order ile Yeni Sipariş  

İlk giriş ekranında terminal seçimi yapıldıktan sonra kullanıcı New Order ekranına yönlendirilir. Bu ekranda sipariş oluşturmak için New Order butonu ve Orders bölümü bulunmaktadır. Orders bölümünde, oluşturulmuş ancak henüz teslim edilmemiş ve teslimat bekleyen siparişler görüntülenebilir.

![orders]({{ '/assets/images/rubyposapp/orders.png' | relative_url }})

New Order butonuna tıklandığında ekrana Section 1'den Section 6'ya kadar farklı bölge seçenekleri ve Live Game seçeneği gelir. Her bölge altında, o bölgeye ait slot makinelerinin numaraları yer alırken Live Game bölümünde masalara isim verilmiştir. Bu yapı sayesinde siparişin gönderileceği slot makinesi veya canlı oyun masası seçilebilir.

![NewOrderPanel]({{ '/assets/images/rubyposapp/NewOrderPanel.png' | relative_url }})

Ekran görüntüsünde görüldüğü gibi, her bölgenin içerisinde o bölgeye ait slot makinelerinin numaraları veya Live Game bölümünde bulunan masa isimleri yer almaktadır.

![bölgeslotnumarası]({{ '/assets/images/rubyposapp/bölgeslotnumarası.png' | relative_url }}) 

## Sipariş verme

Herhangi bir bölgedeki slot makinesi veya Live Game masasının seçilmesinin ardından, siparişin oluşturulacağı menü ve sipariş ekranı açılır. Bu ekranda menü iki ana bölüme ayrılmıştır. Birinci bölümde A La Carte Food menüsü, ikinci bölümde ise sigara ve puro menüsü bulunmaktadır. Kullanıcı, ilgili menüden istediği ürünleri seçerek sipariş oluşturabilir.

![menuekranı]({{ '/assets/images/rubyposapp/menuekranı.png' | relative_url }}) 


## Order list bölümü 

Sayfanın sol tarafında Order List bölümü bulunmaktadır. Bu bölümde, seçilen siparişler listelenir. Ürünlerin yanındaki artı (+) butonu ile ürün adedi artırılabilir, eksi (-) butonu ile azaltılabilir. Ürünlerin sağ tarafında bulunan ilgili ikon kullanılarak ürün adedi iki katına çıkarılabilir.

Bölümün alt kısmında bulunan Close butonu ile bölge ve makine seçim ekranına geri dönülebilir. Clear butonu ile oluşturulan tüm siparişler temizlenebilir. Note butonu kullanılarak ise seçilen ürünlere özel not eklenebilir.

Eğer sipariş verilecek masada daha önceden bir kart takılıysa, Order List bölümü doğrudan ilgili oyuncunun bilgileriyle birlikte açılır. Görselde de görüldüğü gibi, yeni siparişlerin üzerinde ilgili oyuncuya ait Order History bilgileri de görüntülenir. Ayrıca sağda bulunan Add Player butonu ise eğer oyuncu bir makina veya live masada değilse sipariş verdiği zaman isim aratarak siparişi sisteme girilir. Örneğin oyuncu alacart restoranta da sipariş vermek istedi makine veya masa numarası giremeyeceğimiz için böyle bir uygulama yapıyoruz.  

![OrderListNew]({{ '/assets/images/rubyposapp/OrderListNew.png' | relative_url }}) 

## Search kısmı 

Sayfanın sağ tarafında bulunan Search bölümü, ürünlere daha hızlı erişim sağlamak için kullanılabilir. Yemekleri menü içerisinde manuel olarak aramak yerine, ürünün adını Search alanına yazarak ilgili ürüne doğrudan ulaşabilirsiniz.

![FoodSearch]({{ '/assets/images/rubyposapp/FoodSearch.png' | relative_url }}) 

## Next ile garson seçimi 

Sipariş verilecek ürünler seçildikten sonra Next butonuna tıklanır. Bunun ardından sayfanın sağ tarafında yeni bir bölüm açılır ve bu bölümden garson seçimi yapılır. Garson seçimi sayesinde, oluşturulan her siparişin hangi garson tarafından verildiği kayıt altına alınır. Garson seçimi tamamlandıktan sonra sipariş işlemi tamamlanmış olur.

![selectWaiters]({{ '/assets/images/rubyposapp/selectWaiters.png' | relative_url }}) 












