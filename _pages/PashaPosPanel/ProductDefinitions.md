---
title : "Product Definitions"
layout : single 
permalink: /pashapospanel/ProductDefinitions/
---

## Product Definitions Sayfası

### Menu Tablosu 

Menü tablosu, uygulamada bulunan tüm menülerin görüntülendiği ve yönetildiği bölümdür. Bu bölüm üzerinden yeni bir menü oluşturulabilir(yukarda bulunun add a new menü butonundan), mevcut menülere ürün eklenebilir veya menülerde bulunan ürünler güncellenebilir.

Ayrıca mevcut menülerin isimleri değiştirilebilir, menüler güncellenebilir veya artık kullanılmayan menüler silinebilir. Böylece menülerle ilgili tüm düzenleme ve değişiklik işlemleri bu bölüm üzerinden gerçekleştirilebilir.

![MenuTable]({{ '/assets/images/pashapospanel/MenuTable.png' | relative_url }})

Her satırın yanında bulunan Action bölümünde çeşitli butonlar yer almaktadır. Bu butonlar, ilgili menü üzerinde düzenleme, güncelleme ve silme gibi işlemlerin gerçekleştirilmesini sağlar.

- **Update Menu :** Satırın sonunda bulunan Action bölümündeki kalem simgesine tıklandığında, sayfanın sağ tarafında bir panel açılır. Bu panel üzerinden ilgili menünün ismi değiştirilebilir ve yapılan değişiklikler kaydedilebilir.

![UpdateMenu]({{ '/assets/images/pashapospanel/UpdateMenu.png' | relative_url }})

- **Delete Menu :** Action bölümünde bulunan çöp kutusu simgesine tıklandığında, sayfanın sağ tarafında Delete Menu paneli açılır. Bu panel üzerinden seçilen menü silinebilir.

![DeleteMenu]({{ '/assets/images/pashapospanel/DeleteMenu.png' | relative_url }})

- **Menu Product :** Action bölümünde bulunan liste simgesine tıklandığında, sayfanın sağ tarafında Menu Product paneli açılır. Bu panel üzerinden ilgili menüde bulunan ürünler görüntülenebilir ve menüye ürün ekleme veya mevcut ürünleri çıkarma işlemleri gerçekleştirilebilir.

![MenuProducts]({{ '/assets/images/pashapospanel/MenuProducts.png' | relative_url }})

- **Clone Menu :** Action bölümünde bulunan Clone simgesine tıklanarak seçilen menünün bir kopyası oluşturulabilir. Bu özellik, mevcut bir menüyü temel alarak yeni bir menü oluşturmayı kolaylaştırır.

![CloneMenu]({{ '/assets/images/pashapospanel/CloneMenu.png' | relative_url }})

- **Menu Json :** Bu bölümde, ilgili menüye ait JSON detayları görüntülenebilir. JSON verileri sayesinde menü hakkında daha ayrıntılı teknik bilgilere ulaşılabilir ve menünün içerdiği veriler detaylı şekilde incelenebilir.

![MenuJson]({{ '/assets/images/pashapospanel/MenuJson.png' | relative_url }})


### Products Tablosu 

Bu bölüm, uygulamadaki tüm ürünlerin yönetildiği kontrol merkezidir. Yaklaşık 500 ürünün listelendiği bu bölüm üzerinden ürünlerin bilgileri görüntülenebilir, gerektiğinde ürünler silinebilir veya ürün bilgileri düzenlenebilir. Tabloda Product Name, Product Category, Product Tag ve ürünün Favorites bölümünde olup olmadığı gibi bilgiler yer almaktadır.

Her satırda bulunan Action bölümü üzerinden ürünün ismi, kategorisi, Portion Set'i ve Tag'i gibi çeşitli bilgileri değiştirilebilir. Delete seçeneği ile ürün tamamen silinebilir. JSON seçeneği ile ise ürüne ait teknik JSON verileri görüntülenerek daha detaylı inceleme yapılabilir.

Sayfanın üst kısmında, ürünleri daha kolay bulmayı sağlayan detaylı bir Search bölümü bulunmaktadır. Her kategori için ayrı bir arama alanı yer alır. Search bölümünün yanında bulunan Update Multiple ve Delete butonları sayesinde birden fazla ürün aynı anda güncellenebilir veya toplu olarak silinebilir.

![Products]({{ '/assets/images/pashapospanel/Products.png' | relative_url }})

search bölümü ve toplu uptade / delete yeri 

![UstPanelProducts]({{ '/assets/images/pashapospanel/UstPanelProducts.png' | relative_url }})

Action ksımında ürünlerin update edildiği bölüm üzerine bastığınızda sağ tarafda böyle bir panel çıkar ve bu panelden update edilebilir. 

![UpdateProduct]({{ '/assets/images/pashapospanel/UpdateProduct.png' | relative_url }})

### Product Tags Tablosu 

Bu sistemde her ürün bir Product Tag ile ilişkilendirilmiştir. Product Tag'ler, ürünleri belirli gruplar altında sınıflandırmak için kullanılan etiketler olarak düşünülebilir.

Product Tags sayfasında, sistemde bulunan tüm etiketlerin listelendiği bir tablo yer almaktadır. Bu tabloda Product Tag Name, ID ve oluşturulma tarihi gibi bilgiler bulunmaktadır.

Her satırda bulunan Action bölümü üzerinden ilgili Product Tag üzerinde çeşitli işlemler gerçekleştirilebilir. Bu bölüm aracılığıyla Update ve Delete işlemleri yapılabilir. Ayrıca ilgili Product Tag'e ait JSON verileri görüntülenerek teknik detayları incelenebilir.

Bu tablo sayesinde sistemde bulunan Product Tag'ler görüntülenebilir ve etiketlerin isimleri ile diğer bilgileri yönetilebilir.

![ProductTagsTable]({{ '/assets/images/pashapospanel/ProductTagsTable.png' | relative_url }})

### Product Categories Tablosu 

Bu bölüm, menülerde bulunan ürün kategorilerinin yönetildiği bölümdür. Tabloda kategori isimleri ve bazı kategorilerin bağlı olduğu Parent Category bilgileri yer almaktadır.

Tabloda bulunan Action bölümü üzerinden kategoriler üzerinde çeşitli işlemler gerçekleştirilebilir. Bu bölüm aracılığıyla Update ve Delete işlemleri yapılabilir. Ayrıca ilgili kategoriye ait JSON verilerine yine Action bölümünden erişilerek kategori hakkında daha detaylı teknik bilgiler görüntülenebilir.

![ProductCategories]({{ '/assets/images/pashapospanel/ProductCategories.png' | relative_url }})

### Product Portions Table 

Her ürünün, ürüne bağlı olarak farklı Portion seçenekleri bulunabilir. Örneğin Terea ürünü için Turquoise, Purple, Sun Pearl, Silver, Siena, Teak, Yellow, Amber, Mauve ve Wave gibi farklı seçenekler bulunmaktadır. Bu seçenekler sistem içerisinde Portion olarak adlandırılır.

Order Terminal üzerinden sipariş oluşturulurken Terea ürünü seçildiğinde, kullanıcıya bu ürünün mevcut Portion seçeneklerinden birini seçme imkânı sunulur. Ürünlere ait Portion seçenekleri bu bölüm üzerinden yönetilebilir.

Sayfanın üst kısmında bulunan Add a New Portion seçeneği ile yeni bir Portion oluşturulabilir. Her satırda bulunan Action bölümü üzerinden mevcut Portion'lar Update veya Delete seçenekleri kullanılarak güncellenebilir ya da silinebilir. Ayrıca ilgili Portion'a ait JSON verilerine de Action bölümü üzerinden erişilebilir.

![ProductPortionTable]({{ '/assets/images/pashapospanel/ProductPortionTable.png' | relative_url }})

### Portions Table 

Portion Table, sistemde kullanılacak Portion'ların ilk olarak oluşturulduğu ve yönetildiği kontrol merkezidir. Daha önce Product Portion bölümünde bahsedildiği gibi, her ürünün sipariş sırasında seçilebilen kendine özgü Portion seçenekleri bulunabilir.

Bu bölümde yeni Portion'lar oluşturulabilir, mevcut Portion'lar güncellenebilir veya silinebilir. Oluşturulan Portion'lar daha sonra Product Portion tablosu üzerinden ilgili ürünlere atanır.

Kısacası, Portion Table Portion'ların oluşturulduğu ana merkezdir; Product Portion ise oluşturulan bu Portion'ların hangi ürünlere atanacağının yönetildiği bölümdür.

![PortionTable]({{ '/assets/images/pashapospanel/PortionTable.png' | relative_url }})


### Product Extras 

Extra Set bölümü, bazı ürünler için Portion seçeneklerine ek olarak sunulabilecek ekstra seçeneklerin oluşturulduğu ve yönetildiği bölümdür. Örneğin görselde olduğu gibi, bir ürün için Portion seçiminin altında Hellim, Sucuk ve Kaşar gibi ekstra seçenekler sunulabilir.

Yeni bir ürün için ekstra seçenekler tanımlanması gerektiğinde, öncelikle Extra Set Name ile bu seçeneklerin genel adı belirlenir. Daha sonra oluşturulan Extra Set, ilgili ürüne atanır. Böylece kullanıcı sipariş sırasında ilgili ürünü seçtiğinde, Portion seçeneklerinin altında tanımlanan Extra seçenekleri de görüntülenir.

Bu bölüm üzerinden yeni Extra Set'ler oluşturulabilir, mevcut Extra Set'ler düzenlenebilir veya artık kullanılmayan Extra Set'ler silinebilir. Böylece ürünlere sunulacak ekstra seçeneklerin tamamı bu bölüm üzerinden yönetilebilir.

Bu örnekde görebileceğiniz üzere portionsların altında extra olarak seçenek sunuluyor.

![ExampleExtraSet]({{ '/assets/images/pashapospanel/ExampleExtraSet.png' | relative_url }})

Bu görselde extra ların kontrolünü sağladığımız tablo. 

![ProductExtraTable]({{ '/assets/images/pashapospanel/ProductExtraTable.png' | relative_url }})















