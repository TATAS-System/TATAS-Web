# Yayınlama Notları

Bu dosya, siteyi yayınlarken/güncellerken izlenecek adımları ve hatırlatmaları içerir.

## Canlı Site

**https://tatas-system.github.io/TATAS-Web/**

GitHub Pages üzerinden yayınlanıyor — bu repo'ya `main` branch'ine her push yapıldığında site birkaç dakika içinde otomatik güncellenir.

## Bilgisayarında Önizleme

Kurulum gerekmiyor — `index.html` dosyasına çift tıklayıp tarayıcında açman yeterli. Diğer sayfalara üst menüden geçebilirsin.

## GitHub Pages Nasıl Kuruldu (Referans)

1. Bu repo GitHub'da `TATAS-System/TATAS-Web` adıyla **public** olarak oluşturuldu.
2. Repo ayarlarından **Settings → Pages** bölümüne gidildi.
3. "Branch" olarak `main`, klasör olarak `/ (root)` seçilip kaydedildi.
4. Birkaç dakika içinde yukarıdaki canlı link aktif oldu.

Siteyi güncellemek istediğinde: dosyalarda değişiklik yap, `git add`, `git commit`, `git push` — GitHub Pages otomatik olarak yeni sürümü yayınlar.

## Kendi Domainine (tatas-app.com) Bağlama

Domaini satın aldığında:
1. GitHub Pages ayarlarındaki **Custom domain** alanına `tatas-app.com` yaz.
2. Domaini aldığın yerin (GoDaddy, Namecheap vb.) DNS ayarlarına GitHub'ın verdiği adres kayıtlarını (A/CNAME) ekle — GitHub Pages dokümantasyonu bu adımı adım adım anlatıyor.
3. Bağlantı kurulduktan sonra site otomatik olarak `tatas-app.com` üzerinden erişilebilir olur, sayfalardaki linkleri değiştirmene gerek kalmaz (hepsi göreli/relative linkler).

## Güncellemen Gerekenler

- **`index.html`** içindeki "Google Play'de Çok Yakında" butonu — uygulama Play Store'da yayınlandığında, `href="#"` kısmını gerçek Play Store linkinle değiştir (kodda bunu işaret eden bir yorum satırı var).
- **`yasal.html`** — Gizlilik Politikası/Kullanım Koşulları içeriği değişirse, sayfanın en üstündeki "Son güncelleme" tarihini de güncelle.
- **TATAS uygulaması** (`SettingsScreen.tsx`) — Gizlilik Politikası/Kullanım Koşulları linkleri bu siteye (`yasal.html#gizlilik` / `yasal.html#kosullar`) işaret ediyor; domain değişirse orası da güncellenmeli.
