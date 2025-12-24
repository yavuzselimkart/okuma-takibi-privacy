# 📄 Okuma Takibi – Gizlilik Politikası

**Son Güncelleme:** 25 Aralık 2025

Bu Gizlilik Politikası, **Okuma Takibi** (“Uygulama”) tarafından kullanıcı bilgilerinin nasıl işlendiğini, saklandığını ve korunduğunu açıklar.  
Uygulamayı kullanarak bu Gizlilik Politikası’nı kabul etmiş olursunuz.

---

## 📍 1. İzinler ve Kullanım Amaçları

Uygulama, yalnızca temel işlevlerini yerine getirmek için gerekli olan izinleri kullanır.

### 1.1 Kamera İzni
- Kamera izni **yalnızca kullanıcı açıkça fotoğraf çekmeyi başlattığında** kullanılır.
- Kamera **arka planda**, kullanıcıdan habersiz veya otomatik olarak **asla kullanılmaz**.

### 1.2 Galeri / Fotoğraf Seçimi
- Galeriden fotoğraf seçimi **Android Sistem Fotoğraf Seçici (Photo Picker)** üzerinden yapılır.
- Uygulama **READ_MEDIA_\*** izinlerini talep etmez ve kullanıcının tüm fotoğraf veya video arşivine **geniş ya da kalıcı erişim istemez**.
- Yalnızca kullanıcının **bilinçli olarak seçtiği görsellere** erişilir.

### 1.3 Reklam Kimliği (AD_ID)
- Uygulama **Google Mobile Ads (AdMob)** kullanmaktadır.
- Reklam Kimliği (AD_ID), kişiselleştirilmiş veya kişiselleştirilmemiş reklamlar göstermek amacıyla kullanılabilir.
- Reklamlarla ilgili veriler Google’ın kendi gizlilik politikalarına uygun olarak işlenir.

**AdMob Gizlilik Politikası:**  
https://policies.google.com/privacy

### 1.4 Bildirim İzni (Android 13+)
- **Android 13 (API 33)** ve üzeri sürümlerde, Uygulama **POST_NOTIFICATIONS** iznini talep edebilir.
- Bu izin **yalnızca cihaz üzerinde çalışan yerel bildirimler** için kullanılır.
- Bildirimler:
  - Tamamen isteğe bağlıdır
  - Kullanıcı tarafından ayarlanabilir
  - Reklam veya pazarlama amacıyla kullanılmaz
  - Kullanıcı takibi için kullanılmaz
- Uygulama **sunucu tabanlı (push) bildirim göndermez**.

---

## 🖼️ 2. Toplanan Veriler ve Kullanım Amaçları

### 2.1 Kapak Görseli (Fotoğraf)
- Kullanıcı tarafından çekilen veya seçilen kitap kapak görselleri **yalnızca cihaz üzerinde** saklanır.
- Kitap adı, yazar ve sayfa sayısı gibi bilgileri tespit etmek amacıyla, kapak görselinin **base64 formatındaki içeriği**, şifreli bağlantı (HTTPS/TLS) üzerinden aşağıdaki API adresine gönderilir:

https://api.readingtracker.yazilimkodu.com/api/chat/ask

- Görseller yalnızca bu amaçla kullanılır ve **reklam veya pazarlama faaliyetlerinde kullanılmaz**.

### 2.2 Anonim Cihaz Tanımlayıcı (UUID)
- İstekleri sınırlamak ve kötüye kullanımı önlemek amacıyla, Uygulama cihazda **anonim bir UUID** oluşturur.
- Bu UUID, **SharedPreferences** aracılığıyla cihazda saklanır.
- Sunucu ile yapılan isteklerde **başlık (header)** bilgisi olarak gönderilir.
- UUID:
  - Kişisel veri içermez
  - Kullanıcıyı doğrudan tanımlamaz
  - Reklam veya pazarlama amacıyla kullanılmaz

### 2.3 Reklam Verileri
- Google Mobile Ads SDK (AdMob) aşağıdaki verileri işleyebilir:
  - Reklam Kimliği (AD_ID)
  - Cihaz bilgileri
  - Yaklaşık konum ve etkileşim sinyalleri  
  Bu işlemler Google’ın kendi politikalarına tabidir.

### 2.4 Yerel Okuma Hedefi Bildirimleri
- Uygulama, günlük okuma hedeflerini desteklemek amacıyla **yerel bildirimler** oluşturabilir.
- Bildirim davranışları tamamen kullanıcı kontrolündedir ve şunları içerebilir:
  - Bildirim zaman aralıkları
  - Bildirim sıklığı
  - Günlük maksimum bildirim sayısı
- Günlük okuma hedefi tamamlandığında bildirimler **otomatik olarak durur**.
- Hedef tamamlandığında, örneğin şu mesaj gösterilebilir:  
  **“Bugünkü hedefini tamamladın.”**
- Tüm bildirim mantığı **yalnızca cihaz üzerinde** çalışır.
- Bildirimlerle ilgili hiçbir veri sunucuya gönderilmez.

---

## 🔒 3. Veri Saklama ve Silme

- Görseller, bildirim ayarları ve uygulama verileri **yalnızca kullanıcının cihazında** saklanır.
- Uygulama kaldırıldığında, **tüm yerel veriler otomatik olarak silinir**.
- Uygulamada şu özellikler **bulunmamaktadır**:
  - Bulut yedekleme
  - Kullanıcı hesabı
  - Sunucu taraflı kalıcı veri saklama

Bu tür özellikler gelecekte eklenirse, Gizlilik Politikası güncellenecektir.

---

## 🔁 4. Veri Paylaşımı

Uygulama:
- Verileri **pazarlama veya reklam amacıyla satmaz veya paylaşmaz**.

Veriler yalnızca aşağıdaki hizmetlerle, **amaçla sınırlı** olacak şekilde paylaşılır:

1. **Kapak Bilgisi Çıkarma API’si**
   - Paylaşılan veri: Base64 kapak görseli + anonim cihaz UUID
   - Amaç: Kitap bilgilerinin tespiti

2. **Google Mobile Ads (AdMob)**
   - Paylaşılan veri: Reklam ile ilgili veriler
   - Amaç: Reklam gösterimi

---

## 🛡️ 5. Güvenlik

- Sunucu ile yapılan tüm iletişimler **TLS / HTTPS** ile korunur.
- Yetkisiz erişimi ve kötüye kullanımı önlemek için teknik ve idari önlemler alınmıştır.
- Kullanıcılar, veri koruma haklarıyla ilgili talepler için e-posta yoluyla iletişime geçebilir.

---

## 👶 6. Çocukların Gizliliği

- Uygulama **13 yaş altı çocuklar için tasarlanmamıştır**.
- 13 yaş altındaki çocuklardan bilerek kişisel veri toplanmaz.
- Böyle bir durum tespit edilirse, veriler derhal silinir.

---

## 🌍 7. Uluslararası Kullanım ve Kullanıcı Hakları

Uygulama dünya genelinde kullanılabilir.  
Kullanıcılar bulundukları ülkeye göre aşağıdaki haklara sahip olabilir:

- Verilere erişim
- Verilerin silinmesini talep etme
- Veri işlemeye itiraz etme  

(GDPR, KVKK ve benzeri mevzuatlar kapsamında)

---

## 📬 8. İletişim

Bu Gizlilik Politikası ile ilgili her türlü soru ve talep için:

**E-posta:** y.selimkart@gmail.com

---

## ✏️ 9. Değişiklikler

Bu Gizlilik Politikası zaman zaman güncellenebilir.  
Yapılan değişiklikler bu sayfada yayımlandığı anda yürürlüğe girer.  
En güncel tarih her zaman belgenin üst kısmında belirtilir.
