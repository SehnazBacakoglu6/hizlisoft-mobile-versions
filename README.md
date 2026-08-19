# HızlıSoft Mobile App Versions

HızlıSoft mobil uygulamalarının Android ve iOS sürüm bilgilerinin merkezi olarak tutulduğu repository'dir.

Mobil uygulamalar, güncelleme kontrolü sırasında bu repository içerisindeki `versions.json` dosyasını kullanır.

## 📱 Uygulamalar

- HızlıSoft Saha Satış
- HızlıSoft Kiosk Satış
- HızlıSoft Fiyat Gör
- HızlıBoss
- HızlıSoft Mutfak
- HızlıSoft Garson
- HızlıSoft Sıramatik

## 📄 versions.json

`versions.json` dosyasında her uygulamanın Android ve iOS platformlarına ait güncel sürüm bilgileri bulunur.

Her platform için:

- `versionCode` / `build` → Teknik sürüm numarası
- `versionName` / `marketingVersion` → Kullanıcıya gösterilen sürüm
- `storeUrl` → Google Play veya App Store bağlantısı

bilgileri tutulur.

## 🔄 Güncelleme Kontrolü

Mobil uygulama açıldığında `versions.json` dosyasını kontrol eder.

Örneğin:

```text
Yüklü sürüm
     ↓
versions.json
     ↓
Yeni sürüm var mı?
     ↓
   ┌───────┐
   │       │
  Hayır   Evet
   │       │
 Devam   Güncelleme
           ↓
      Mağazayı Aç
