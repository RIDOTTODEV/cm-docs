---
title: "Settings"
layout: single
permalink: /pashaposkiosk/settings/
--- 

## Settings

Settings bölümü, uygulamaya ait çeşitli ayarların görüntülendiği ve düzenlendiği bölümdür.

- **Security** - : Uygulama ayarlarında yapılan değişikliklerin kaydedilmesini sağlayan bölümdür. Yapılan değişikliklerin kaydedilebilmesi için Save Terminal Settings seçeneğinin açık olması gerekmektedir.


![Security]({{ '/assets/images/pashaposkiosk/Security.png' | relative_url }})

- **Waiting Orders** - : Bu bölümde Sort By State, Tags, Restore, Ask Password for Restoring ve Section ile ilgili çeşitli ayarlar bulunmaktadır.

**Sort By State:**: Siparişlerin Order History bölümünde durumlarına göre sıralanmasını sağlar.

**Tags**: Siparişlerin oluşturulduğu terminalde, menüde hangi kategorilerin görüntülenip görüntülenmeyeceğini belirler.

**Restore**: Bu seçenek açık olduğunda, verilen siparişlerin Attend Terminal üzerinden silinmesine olanak sağlar.

**Ask Password for Restoring**: Sipariş silme işlemi sırasında şifre sorulmasını sağlar. Örneğin, Restore ve Ask Password for Restoring seçenekleri açık olduğunda, sipariş silinirken kullanıcıdan şifre girmesi istenir.

**Section** : Terminalde hangi bölgelerin görüntüleneceğini belirlemek için kullanılır. Bir bölge devre dışı bırakıldığında, o bölgeye ait siparişler ilgili terminalin Orders bölümünde görüntülenmez. Bu sayede her terminalde yalnızca ilgili bölgelere ait siparişlerin gösterilmesi sağlanarak siparişlerin karışması önlenir.

![waitingorders]({{ '/assets/images/pashaposkiosk/waitingorders.png' | relative_url }})

- **New Order** - : Yeni bir sipariş oluşturulduğunda bildirim sesi çalmasını sağlayan ayardır. Bu seçenek kullanılarak sipariş oluşturulduğunda çalan bildirim sesi açılabilir veya kapatılabilir.

![NewOrder]({{ '/assets/images/pashaposkiosk/NewOrder.png' | relative_url }})

- **Environments** - : Bu ayar bölümünde arayüzün çalışmasıyla ilgili çeşitli API URL bilgileri bulunmaktadır. Player last order count dediği şey ise oyuncunun en son kaç siparişini göstereceğini belirler.

![Environments]({{ '/assets/images/pashaposkiosk/Environments.png' | relative_url }})

- **Info** - : Bu bölümde uygulama ve terminal hakkında çeşitli bilgiler yer almaktadır. Terminal Name, Terminal UUID, Menu Names, Login User Name ve Application Version gibi bilgiler bu bölüm üzerinden görüntülenebilir.

![info]({{ '/assets/images/pashaposkiosk/info.png' | relative_url }})




