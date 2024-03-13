### Proje Tanımı ve Fonksiyonlar

Bu projede, bir ATM simülasyonu geliştireceğiz. Kullanıcıların giriş yapmasını, hesap bakiyelerini sorgulamasını, para çekip yatırmasını ve hesap bilgilerini görüntülemesini sağlayacak bir dizi fonksiyon oluşturacağız. Aşağıda projenin temel bileşenleri ve fonksiyonların detayları verilmiştir:

1. **`para_cek(hesap, miktar)` Fonksiyonu:**
   - Kullanıcının hesabından belirli bir miktar para çekmesini sağlar.
   - Hesap bakiyesi ve ek hesap limiti yeterliyse, işlemi gerçekleştirir ve yeni bakiyeyi gösterir.

2. **`giris_yap(username, password)` Fonksiyonu:**
   - Kullanıcı adı ve şifre ile giriş yapmayı sağlar.
   - Giriş başarılıysa, kullanıcıya ait hesap bilgilerini döndürür.

3. **`bakiye_sorgu(hesap)` Fonksiyonu:**
   - Kullanıcının mevcut bakiyesini ve ek hesap limitini gösterir.

4. **`hesap_bilgi(hesap)` Fonksiyonu:**
   - Hesaba ait tüm bilgileri yazdırır. (Örn: Kullanıcı adı, bakiye, ek hesap limiti vs.)

5. **`para_yatir(hesap, yatirim)` Fonksiyonu:**
   - Kullanıcının hesabına para yatırmasını sağlar.
   - Eğer ek hesap kullanılmışsa, öncelikle ek hesap bakiyesini tamamlar, sonra ana bakiyeyi artırır.

### Ana Ekran Fonksiyonu

`ana_ekran()` fonksiyonu ile kullanıcıların ATM işlemlerini yöneteceğiz. Bu fonksiyon, aşağıdaki adımları içerir:

- **Giriş Yapma:**
  - `giris_yap` fonksiyonunu kullanarak kullanıcı girişi yapılmasını sağlar.
  - Başarılı giriş sonrası, kullanıcıya işlem seçenekleri sunulur.
  - 3 başarısız giriş denemesinden sonra erişim engellenir.

- **İşlem Seçenekleri:**
  - Kullanıcıdan işlem türü seçmesi istenir:
    1. Para Çekme
    2. Para Yatırma
    3. Bakiye Sorgulama
    4. Hesap Bilgileri
    5. Çıkış

### Modüller

- **islem Modülü:**
  - `giris_yap`, `para_cek`, `bakiye_sorgula`, `para_yatir`, ve `hesap_bilgi` fonksiyonlarını içerir.

- **hesap Modülü:**
  - Kullanıcı adları listesi ve her bir kullanıcıya ait hesap bilgilerini (dict formatında) tutar.






