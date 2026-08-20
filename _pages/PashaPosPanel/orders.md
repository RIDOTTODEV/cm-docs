---
title: "Orders"
layout: single 
permalink: /pashapospanel/orders/
---

## Orders Sayfası 

Bu sayfada tüm orderlarin teslim edilmiş veya edilmemiş hepsinin listelendiği bölümdür 

Sayfanın üst kısmında, siparişleri belirli kriterlere göre filtrelemeyi sağlayan Filter bölümü bulunmaktadır. Bu bölümde Section, Table, Waiter ve Statuses gibi temel filtreleme araçları yer alır.

- **Section :** Seçilen bölgeye ait siparişlerin listelenmesini sağlar.
- **Table :** Seçilen masa adına ait siparişleri listeler. Buradaki masa adı, slot makinesi numarası veya oyuncu adı olabilir.
- **Waiter :** Belirli bir garson seçilerek, yalnızca o garson tarafından oluşturulan siparişlerin listelenmesini sağlar.
- **Statuses :** Siparişleri durumlarına göre filtreler. Bu seçenek üzerinden teslim edilmiş, yeni veya iptal edilmiş siparişler ayrı ayrı görüntülenebilir.

Show More butonuna tıklandığında daha fazla filtreleme seçeneği açılır:

- **Player :** Oyuncu adı girilerek ilgili oyuncuya ait siparişlerin bulunmasını sağlar.
- **Product Tag :** Belirli bir ürün etiketine göre siparişlerin filtrelenmesini sağlar.
- **Product Name :** Belirli bir ürün adına göre siparişlerin listelenmesini sağlar.
- **Completed :** Yes seçildiğinde teslim edilmiş siparişler, No seçildiğinde ise henüz teslim edilmemiş siparişler listelenir.

Bu filtreleme seçenekleri sayesinde sayfada tüm geçmiş siparişler görüntülenebildiği gibi, farklı filtreler kullanılarak belirli kriterlere uyan siparişler de hızlı bir şekilde bulunabilir.

![filter]({{ '/assets/images/pashapospanel/filter.png' | relative_url }})

## Orders Tablosu 

Filtreleme kısmının altında orders tablosu bulunur burada en yeni siparişden en eski siparişe göre listelendiği yerdir kioskda her yeni sipariş eklendiğinde burası da yenilenir ve bu listeye düşer yine bu tablonunda kendi içinde search yeri vardır ve arama için sipariş İd , terminal ismi, table numarası veya ismi ve waiter ismi girilmelidir. ayrıca search bölümünün yanında refres butonunu yeni sipariş geldiğinde tabloyu refres etmesi için tabloyu tam ekrana almak için tam ekran butonu ve dilediğinizde listeyi indirmek için export simgesi bulunmaktadır. 

![orderstablosu]({{ '/assets/images/pashapospanel/orderstablosu.png' | relative_url }})

## JSON Details bölümü

Tabloda her satırın sonunda action bölümü var bu bölümün amacı her siparişin json kodlarına buradan ulaşabilirisiniz. Bu JSON kodlarına bakarak aslında siparişin nereden geldiği, kimin oluşturduğu, hangi masaya ait olduğu, ne ürün söylendiği ve siparişin hangi durumda olduğu hakkında oldukça fazla şey çıkarabiliriz.

![Jsonkodları]({{ '/assets/images/pashapospanel/Jsonkodları.png' | relative_url }})







