# TDA QR

TDA QR, tarayıcıda QR kodu oluşturup görsel olarak indirmeye yarayan tek sayfalı bir web uygulamasıdır. Kaynak dosyalar `index.html` ve `TDA_Logo.png` dosyalarıdır.

## Özellikler

- URL, düz metin veya Wi-Fi bağlantı bilgisi için QR kodu oluşturur.
- Wi-Fi ağı için WPA/WPA2, WEP veya şifresiz ağ seçeneklerini destekler; gizli ağ seçeneği de vardır.
- QR kodunun ön plan ve arka plan renklerini özelleştirir.
- İsteğe bağlı PNG, JPEG veya WebP logo ekler ve logoyu QR kodunun ortasında kullanır.
- QR kodunu PNG olarak 800 × 800, 1200 × 1200 veya 1600 × 1600 pikselde indirir.
- Açık/koyu tema sunar.

Logolu QR kodu paylaşmadan önce farklı telefon ve tarayıcılarla okutmayı dene. Büyük logo veya düşük kontrast kodun okunmasını zorlaştırabilir.

## Çalıştırma

1. Depoyu indir veya klonla.
2. `index.html` ile `TDA_Logo.png` dosyalarını aynı klasörde tut.
3. `index.html` dosyasını güncel bir tarayıcıda aç.

QR oluşturma kodu tarayıcıda çalışır; uygulama QR içeriği için kendi sunucusuna istek yapmaz. Ancak görünüm ve QR kütüphanesi `cdn.tailwindcss.com` ile jsDelivr CDN’inden yüklenir; ilk açılışta bu dosyaları almak için internet bağlantısı gerekir. CDN erişimi yoksa stil veya QR üretimi çalışmayabilir.

## Dağıtım

`index.html` ve `TDA_Logo.png` birlikte statik web barındırıcısına yüklenmelidir. Depo `tda_qr` için Apache License 2.0 bildiriyor. Üçüncü taraf kütüphaneler ve bileşenler kendi lisans bildirimlerine tabidir; yeniden dağıtımda bunların şartlarını da koru.

## Sınırlar

Wi-Fi QR kodunu okuyan cihazın ağa otomatik bağlanma teklifi, o cihazın işletim sistemi ve QR okuyucusuna bağlıdır. Uygulama cihazın bağlantısını kendisi kurmaz. İndirdiğin görseli dağıtmadan veya baskıya göndermeden önce kodun okunabilirliğini doğrula.
