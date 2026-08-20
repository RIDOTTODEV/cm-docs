---
title : "Settings"
layout : single
permalink : /pashapospanel/Settings/
---

## Settings 

Bu sayfa, Pasha POS Panel uygulamasına ait genel ayarların yönetildiği bölümdür. Ayarlar kendi içerisinde Email Settings ve Other Settings olmak üzere iki ana bölüme ayrılmıştır.

### Email Settings

Bu bölüm, sistemin e-posta gönderimi için kullandığı temel e-posta ayarlarının yönetildiği alandır. Burada e-posta adresi, SMTP Host, şifre ve port gibi bağlantı bilgileri tanımlanır. Bu ayarlar, sistemin e-posta servisleriyle doğru şekilde iletişim kurabilmesi için kullanılır.

![EmailSettings]({{ '/assets/images/pashapospanel/EmailSettings.png' | relative_url }})

### Other Settings

**Other Settings** bölümü, sistemin daha detaylı ve genel ayarlarının yönetildiği bölümdür. Bu bölümde farklı sistem ve kullanıcı işlemleriyle ilgili çeşitli ayarlar bulunmaktadır.

* **Gaming Date Turn Hour:** Sistemde bir günün hangi saatte değişeceğini belirler. Örneğin saat **07:00** olarak ayarlanmışsa, yeni gün gece 00:00'da değil, sabah 07:00'de başlar. Bu nedenle 00:00–07:00 arasındaki işlemler önceki gaming date'e dahil edilir.

* **Attendant Order Delete Password:** Terminal uygulamasında bulunan **Restore** işlemleri ile bir siparişin silinebilmesi için gereken şifredir. Siparişlerin silinmesi veya geri alınması gibi işlemler için yetkili kullanıcıların şifre girmesi gerekir.

* **Inspector Order Delete Password:** Inspector kullanıcılarının sipariş silme işlemlerinde kullanacağı şifre burada belirlenir.

* **Ridotto API URL:** Ridotto API bağlantısında kullanılan URL bilgisinin yönetildiği alandır. API adresi değiştiğinde buradan güncellenebilir.

* **Ridotto API User:** Ridotto API bağlantısı için kullanılan kullanıcı bilgilerinin girildiği alandır.

* **Ridotto API Password:** Ridotto API bağlantısında kullanılan şifrenin tanımlandığı alandır.

* **Assist API URL:** Assist API bağlantısında kullanılan URL bilgisinin yönetildiği alandır. URL değişiklikleri bu bölümden yapılabilir.

* **Inspector Terminal UUID:** İnspector un hangi terminali kullanacağını belirler

* **Attendant Terminal UUID:** Attendant un hangi terminali kullanacağını belirler 

Bu bölümde bulunan URL, kullanıcı adı ve şifre gibi bağlantı bilgileri, ilgili servislerin sistem tarafından doğru şekilde kullanılabilmesi için kontrol edilir ve gerektiğinde güncellenebilir.


![OtherSettings]({{ '/assets/images/pashapospanel/OtherSettings.png' | relative_url }})

 



