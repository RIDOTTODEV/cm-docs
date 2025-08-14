---
title: "Ridotto Kurulumu"
parent: "Ridotto"
layout: single
nav_order: 1
permalink: /ridotto/kurulum/
# parent alanı üst sayfa ile bağlantıyı kurar.
# nav_order ile sıralama yaparsın.
---

# Ridotto Casino Yönetim Sistemi - Kurulum Kılavuzu

Bu döküman, Ridotto sisteminin ilk kurulum sürecini ve gerekli bileşenlerin tanımlanmasını anlatır.

---

## 1. Yazılım Kurulumu

    **Sunucu Tarafı**

- Sunucuda güncel docker yazılımını kurun.
- Ridotto docker yml dosyalarını yükleyin sunucuya göre yapılandırın.
- Github üzerinden oluşturulan login token ı ile aşağıdaki gibi giriş yapın:

  ```bash
  docker login ghcr.io -u USERNAME
  ```

---

## 2. SMIB Cihazlarının Kurulumu

1. **SMIB Donanım Montajı**
   - Slot makinesinin uygun bağlantı portuna takın.
   - Güç bağlantısını yapın.
   - Ethernet kablosu ile ağ bağlantısını sağlayın.

2. **SMIB Yazılım Tanımlaması**
   - Ridotto yönetim paneline giriş yapın.
   - **Makine Yönetimi > Slot Makinesi Tanımla** menüsüne gidin.
   - Slot Makinesine dair bilgileri ve cihazın mac adres ve port numaralarını doğru tanımlayın.
   - SMIB cihazı başlatın ve sistem hazır

---

## 3. İlk Konfigürasyon

- **Kullanıcı Rolleri**: Yönetici, Supervisor, Operatör, Rapor Görüntüleyici
- **Makine Grupları**: Bölge, Salon, Ada bazlı gruplama
- **Oyun Profilleri**: Slot makinesi yazılım sürümleri ve temalar

---

## 4. Test & Doğrulama

- Test oyuncu ile oturum açın.
- Makineye oturma/kalkma işlemini deneyin.
- Rapor ekranında veri akışını kontrol edin.

