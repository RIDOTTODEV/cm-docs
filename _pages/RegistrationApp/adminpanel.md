---
title: "Admin Panel"
layout: single
permalink: /registrationapp/adminpanel/
---

## Registration App Admin Panel

Admin panel sayfası Registration App uygulamasının API URL,SERVICE URL ve benzeri hassas ayarlamalarının yapıldığı yönetici panelidir.

## Genel Kullanım Ve Sayfa Düzeni

Registration App Admin Panele erişmek için sol üst köşedeki Pasha Card Desk Başlığının DESK kısmına 2 kez tıklanır.

![AdminPanelLoginPage]({{ '/assets/images/registrationapp/AdminPanelLoginPage.png' | relative_url }})

Önümüze çıkan sayfadaki kutucuğa admin şifresi yazılır ve giriş yapılır.

![PasswordPage]({{ '/assets/images/registrationapp/PasswordPage.png' | relative_url }})

Admin panele giriş yaptığımızda bizi Ayarlar sayfası karşılar. Bu sayfada aşağıdaki ayarlar bulunur:

- **Kart Basım Ayarları** — Kart üzerine basılan ismin hizalanması ve boyutlandırılması
- **API URL** — Registration App'in verileri hangi sunucudan çekeceğinin ayarı
- **Card Desk Service URL** — Card Desk servisinin çalıştığı URL adresi
- **Yasal Sözleşme Ayarları** — Bulgaristan'da yürürlükte olan ve gelen misafirlerin bilgilerinin gerektiğinde     paylaşılabileceğini belirten kanuni sözleşme metni ayarı
- **Printer Ayarları** — Registration App'in çıktıyı hangi yazıcıdan alacağının ayarı

![TopSettings]({{ '/assets/images/registrationapp/TopSettings.png' | relative_url }})

Buranın hemen altında ise varsayılan olarak tarih filtrelemesinin başladığı gün ve saat ayarı yapılır ve varsayılan olarak 07:00 atanmıştır (salı günü saat 07:00 ile çarşamba günü saat 07:00 arasındaki misafirleri 1 gün olarak listelememizi sağlar).

![DateSettings]({{ '/assets/images/registrationapp/DateSettings.png' | relative_url }})

Alt kısımda bulunan onay kutuları, birkaç özelliği aktif veya deaktif etmemizi sağlar:

- **İmza Kullanımı** — Bulgaristan'da canlı olarak kullanılan ve gerektiğinde bilgi paylaşımının resmi olarak gerçekleştirilmesini sağlayan onay formu imzası
- **Ek Bilgi Uyarıları** — Casinoya giriş yapmış misafirlerin eksik dokümanlarını kullanıcıya uyarı olarak gösterme
- **Yanlış Belge Silme Yetkisi**

![MiddleSettings]({{ '/assets/images/registrationapp/MiddleSettings.png' | relative_url }})

Onay kutularının hemen alt kısmında ise Check-In durumları adında bir bölüm bulunur burada misafirleri grupladığımız etiketlerimizi yaratabilir isim ve renklerini belirleyebiliriz.

![TagSettings]({{ '/assets/images/registrationapp/TagSettings.png' | relative_url }})

Alt kısımda ise imza formu için sisteme cihaz bağlama kısmı ve Kaydet butonu bulunmaktadır.

Ekranın en sağ alt köşesinde ise ilk defa kurum yapılacak cihazlarda varsayılan ayarları yüklemesi için bir reset to default butonu bulunmaktadır.
