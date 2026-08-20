---
title : "Definitions"
layout : single 
permalink: /pashapospanel/Definitions/
---

## Definitions

### Sections 

Sipariş oluşturma sırasında Section 1'den Section 6'ya kadar olan bölgeler ve Live Game seçeneği kullanılmaktadır. Section bölümü, bu bölgelerin yönetildiği ve kontrol edildiği bölümdür.

Bu sayfa üzerinden yeni bir Section eklenebilir, mevcut Section'lar güncellenebilir veya artık kullanılmayan Section'lar silinebilir. Bu nedenle Section'ların oluşturulması ve yönetilmesiyle ilgili tüm işlemler bu bölüm üzerinden gerçekleştirilir.

![SectionTable]({{ '/assets/images/pashapospanel/SectionTable.png' | relative_url }})

### Tables Name 
 
Tables bölümü, sistemde bulunan masa ve slot makinelerinin yönetildiği bölümdür. Bu bölüm üzerinden yeni bir masa oluşturulabilir ve oluşturulan masa istenilen bir Section'a atanabilir. Böylece oluşturulan masa, sipariş oluşturma ekranında ilgili bölge içerisinde görüntülenir.

Slot makinelerinin numaraları ve Live Game bölümünde bulunan masa isimleri bu bölüm üzerinden yönetilir. Mevcut masalar Update seçeneği ile güncellenebilir veya artık kullanılmayan masalar Delete seçeneği ile silinebilir.

Örneğin, Section 1 içerisinde Slot 999 adında yeni bir masa oluşturulabilir. Daha sonra bu masanın numarası Slot 991 olarak güncellenebilir veya masa artık kullanılmıyorsa sistemden silinebilir. Ayrıca oluşturduğunuz bir masa belirli bir sectiona bağlı olmayabilir. 

![TableName]({{ '/assets/images/pashapospanel/TableName.png' | relative_url }})

### Terminals 

Terminal, siparişlerin girildiği kioskları ifade eder. Casinoda siparişlerin tek bir noktadan alınması yerine, farklı bölümlere ayrılmış birden fazla terminal bulunmaktadır. Bu terminallere Casino Bar, Ana Restoran, Slot gibi isimler verilmiştir.

Her terminal, bulunduğu bölüme özel menülere sahip olabilir. Örneğin, Ana Restoran terminalinde yalnızca alakart menüler bulunurken, Slot terminalinde yalnızca sigara menüleri bulunabilir.

Bu bölümde, her terminal için kullanılacak menüler tanımlanır ve ilgili terminale atanır. Bir terminale birden fazla menü atanabilmektedir. Böylece her sipariş noktasında yalnızca o bölümü ilgilendiren menülerin kullanılabilmesi sağlanır.

![Terminals]({{ '/assets/images/pashapospanel/Terminals.png' | relative_url }})

### Printers

Bu sayfa printer lerin kontrolu için kullanılan tablodur bu sayfadan printers ekleyebilir veya silebilir yada update edebilirsiniz.  

![Printers]({{ '/assets/images/pashapospanel/Printers.png' | relative_url }})

Printer eklerken veya mevcut bir printer'ı güncellerken bir ayar menüsü açılır. Bu menüde öncelikle printer'ın adı, IP adresi ve MAC adresi girilir.

Daha sonra printer'ın hangi Tag, Menu ve Section bilgilerini kapsayacağı belirlenir. Bu alanlar sayesinde kullanıcılar printer'ları belirli kriterlere göre sınıflandırabilir. Örneğin, yalnızca belirli menülerde bulunan ürünlerin veya belirli bir bölgeden gelen siparişlerin ilgili printer'da yazdırılması sağlanabilir.

Tüm ayarlar tamamlandıktan sonra Save butonuna tıklanarak yapılan değişiklikler kaydedilir.

![AddaNewPrinter]({{ '/assets/images/pashapospanel/AddaNewPrinter.png' | relative_url }})


### Waiters 

Bu sayfada, sipariş girerken Terminal uygulamasında karşımıza çıkan garson seçimi için kullanılan garsonlar yönetilir. Bu bölüm üzerinden yeni bir garson eklenebilir, mevcut garsonların bilgileri güncellenebilir veya garsonlar silinebilir.

![WaitersTable]({{ '/assets/images/pashapospanel/WaitersTable.png' | relative_url }})

Yeni bir garson eklerken garsonun adı, soyadı, doğum tarihi, PIN kodu, şifresi ve bağlı olduğu terminal bilgileri girilir. Terminal seçimi sayesinde her terminal için farklı garsonlar tanımlanabilir.

Formun en altında, garsonun Captain olup olmadığını belirleyen bir seçenek bulunur. Garson Captain ise bu seçenek aktif bırakılır. Captain olarak tanımlanan garsonlara, sigara siparişleri için onay gönderilir. Sigara siparişlerinin onay süreciyle ilgili detaylı bilgiye ilgili panelin dokümantasyonundan ulaşabilirsiniz.

Tüm bilgiler girildikten veya gerekli değişiklikler yapıldıktan sonra Save butonuna tıklanarak ayarlar kaydedilir.

![AddaNewWaiter]({{ '/assets/images/pashapospanel/AddaNewWaiter.png' | relative_url }})




