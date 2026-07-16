# TATAS-Web

TATAS uygulamasının tanıtım sitesi. Herhangi bir kurulum/derleme (build) gerektirmez — sadece düz HTML/CSS dosyalarından oluşur, bir tarayıcıda doğrudan açılabilir veya herhangi bir statik dosya barındırma servisine olduğu gibi yüklenebilir.

## Dosya Yapısı

```
TATAS-Web/
├── index.html               Ana Sayfa (tanıtım + indirme linki)
├── kullanim-kilavuzu.html   Adım adım kullanım rehberi + SSS
├── yasal.html                Gizlilik Politikası + Kullanım Koşulları
├── css/style.css            Tüm sayfaların paylaştığı tek stil dosyası
└── img/                      Uygulama simgesi (uygulamanın kendi assets klasöründen kopyalandı)
```

## Bilgisayarında Önizleme

Kurulum gerekmiyor — `index.html` dosyasına çift tıklayıp tarayıcında açman yeterli. Diğer sayfalara üst menüden geçebilirsin.

## Yayınlama (İlk Kez Yapıyorsan)

En kolay ve ücretsiz yol **GitHub Pages**:

1. [GitHub](https://github.com) hesabın yoksa ücretsiz bir tane oluştur.
2. Yeni bir repository (depo) oluştur, adını `tatas-web` gibi bir şey koy.
3. Bu klasördeki (`TATAS-Web`) tüm dosyaları o depoya yükle (GitHub'ın web arayüzündeki "Add file → Upload files" ile sürükle-bırak yapabilirsin, komut satırı gerekmez).
4. Depo ayarlarından **Settings → Pages** bölümüne git, "Branch" olarak `main` seçip kaydet.
5. Birkaç dakika içinde sana `https://kullanici-adin.github.io/tatas-web/` gibi bir link verilecek — bu senin canlı sitenin adresi.

## Kendi Domainine (tatas-app.com) Bağlama

Domaini satın aldığında:
1. GitHub Pages ayarlarındaki "Custom domain" alanına `tatas-app.com` yaz.
2. Domaini aldığın yerin (GoDaddy, Namecheap vb.) DNS ayarlarına GitHub'ın verdiği adres kayıtlarını (A/CNAME) ekle — GitHub Pages dokümantasyonu bu adımı adım adım anlatıyor.
3. Bağlantı kurulduktan sonra site otomatik olarak `tatas-app.com` üzerinden erişilebilir olur, `index.html` içindeki linkleri değiştirmene gerek kalmaz.

## Güncellemen Gerekenler

- **`index.html`** içindeki "Google Play'de Çok Yakında" butonu — uygulama Play Store'da yayınlandığında, `href="#"` kısmını gerçek Play Store linkinle değiştir (kodda bunu işaret eden bir yorum satırı var).
- **`yasal.html`** — Gizlilik Politikası/Kullanım Koşulları içeriği değişirse, sayfanın en üstündeki "Son güncelleme" tarihini de güncelle.
