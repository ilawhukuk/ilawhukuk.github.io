# iLaw Hukuk: web sitesi

Bu klasör herkese açık sitenin kaynağıdır. Yayın: `ilawhukuk/ilawhukuk.github.io` deposu, GitHub Pages (`main` dalı, kök)
→ https://ilawhukuk.github.io/

Değişiklik uygulamanın asıl (özel) deposunda yapılır; sonra bu klasörün tamamı, `.nojekyll` ve `.well-known/` dahil, yayın
deposuna kopyalanır.

| Dosya | Görev |
| --- | --- |
| `index.html` | Ana sayfa |
| `gizlilik.html` | Gizlilik Politikası |
| `aydinlatma.html` | Aydınlatma Metni (KVKK m.10) |
| `kosullar.html` | Kullanım Koşulları; uygulamadaki koşul sürümü bu sayfanın tarihidir |
| `hesap-silme.html` | Hesap silme: adımlar, silinen ve saklanan veriler, süreler (mağazalara verilen adres) |
| `kunye.html` | İletişim ve künye |
| `indir.html` | Uygulamayı edinme; uygulamadaki "Yeni sürümü indir" buraya açılır |
| `davet.html`, `kisi.html` | Meslektaş daveti ve kişi bağlantısı: uygulama kuruluysa uygulamada açılır, değilse İndir sayfasına gider |
| `surum.json` | Uygulamanın okuduğu sürüm ayarı: `latest`, `minVersionCode`, `downloadUrl`, `testEndsAt`, `notice` (iPhone için `ios`) |
| `.well-known/assetlinks.json` | Android'in doğrulanmış bağlantıları (Play'deki uygulama) |
| `icon.png`, `favicon.png` | Uygulama simgesinden küçültülmüş |
| `.nojekyll` | GitHub Pages dosyaları olduğu gibi sunar |
| `dene/` (bu klasörde değil) | Web deneme sürümü; asıl depoda `bash scripts/web-deneme.sh` ile üretilir, yayın deposuna ayrıca konur |

- Gizlilik, aydınlatma, koşullar, hesap silme ve künye sayfaları taslaklarından üretilir; burada elle düzeltilmez.
- Gizlilik metni uygulamanın gerçek veri akışını anlatır. Veri akışı değişirse metin de değişir.
- Eski site adresi bu siteye yönlendirir. Eski kurulumlar sürüm ayarını oradaki `surum.json`'dan okuduğu için o dosya
  gerçek dosya olarak kalır ve bununla aynı tutulur.
