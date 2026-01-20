# Headless Browser Automation Tespiti ve Kaçınma Teknikleri

**Kaynak Proje:** [https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation](https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation)

---

## 1. Temel Çalışma Prensipleri

Headless browser automation, bir tarayıcının grafik arayüzü olmadan (headless mode) çalıştırılarak web sayfalarının programatik olarak kontrol edilmesini sağlar. Selenium, Puppeteer ve Playwright gibi araçlar bu yaklaşımın en yaygın örnekleridir.

Modern web siteleri, bot trafiğini tespit etmek için çok katmanlı fingerprint ve davranış analizleri kullanır. Bu projede, özellikle aşağıdaki tespit sinyallerine odaklanılmıştır:

### 1.1 Bot Tespit Sinyalleri

* `navigator.webdriver` değerinin `true` olması
* Headless Chrome’a özgü User-Agent paterni
* Plugin ve font eksiklikleri
* Canvas ve Audio fingerprint anomalileri
* WebGL vendor / renderer tutarsızlıkları
* Mouse ve klavye etkileşiminin olmaması
* Scroll davranışı eksikliği
* Timing pattern farklılıkları
* Proxy ve IP reputation

### 1.2 Kaçınma (Evasion) Teknikleri

Repo’da yer alan teknikler, bu sinyallerin maskelemesini veya normalize edilmesini amaçlar:

* `navigator.webdriver` override edilmesi
* Headless flag’lerinin devre dışı bırakılması
* Gerçekçi User-Agent kullanımı
* Sahte plugin ve font enjeksiyonu
* Canvas ve WebGL fingerprint normalizasyonu
* İnsan benzeri mouse ve scroll event simülasyonu
* Locale, timezone ve dil ayarlarının eşitlenmesi

Bu teknikler, bot tespit sistemlerinin fingerprint tabanlı sınıflandırma modellerini yanıltmayı hedefler.

---

## 2. Best Practices ve Endüstri Standartları

Headless browser automation kullanırken aşağıdaki en iyi uygulamalar önerilir:

### 2.1 Tarayıcı Yapılandırması

* Headless yerine headed mode veya stealth mode kullanmak
* User-Agent ve viewport değerlerini sabitlemek
* `--disable-blink-features=AutomationControlled` flag’i kullanmak
* Chrome infobar ve automation flag’lerini kapatmak

### 2.2 Davranış Simülasyonu

* Gerçekçi mouse hareketleri üretmek
* Rastgele scroll davranışı eklemek
* Sayfa yüklenme sürelerine uygun bekleme süreleri kullanmak
* Klavye girişleri ve form doldurma simülasyonu

### 2.3 Fingerprint Yönetimi

* Canvas fingerprint maskesi
* WebGL vendor / renderer spoofing
* AudioContext fingerprint normalizasyonu
* Plugin ve font listesi enjeksiyonu

### 2.4 Proxy ve IP Yönetimi

* Residential veya mobile proxy kullanmak
* IP rotation uygulamak
* ASN reputation kontrolü
* Rate-limit davranışı oluşturmak

### 2.5 Endüstride Yaygın Stealth Araçları

* puppeteer-extra-plugin-stealth
* undetected-chromedriver
* playwright-stealth
* Selenium Stealth

---

## 3. Benzer Açık Kaynak Projeler ve Rakipler

Bu proje, bot tespit ve kaçınma alanında yer alan diğer açık kaynak çözümlerle benzer hedeflere sahiptir:

### 3.1 Açık Kaynak Projeler

* **puppeteer-extra-plugin-stealth**
  Headless Chrome fingerprint’lerini maskeleyen popüler bir Puppeteer eklentisi.

* **undetected-chromedriver**
  Selenium için stealth Chrome driver implementasyonu.

* **playwright-stealth**
  Playwright üzerinde fingerprint spoofing sağlayan paket.

* **Selenium Stealth**
  Selenium tabanlı stealth script koleksiyonu.

### 3.2 Tespit Tarafı Araçları

* **FingerprintJS**
  Canvas, Audio, WebGL ve tarayıcı fingerprint üretimi.

* **PerimeterX / Human / Akamai Bot Manager**
  Endüstride yaygın kullanılan bot tespit çözümleri.

---

## 4. Kritik Yapılandırma Dosyaları ve Parametreler

Headless browser automation’da başarı için yapılandırma parametreleri kritik öneme sahiptir.

### 4.1 Chrome Flags

* `--disable-blink-features=AutomationControlled`
* `--no-sandbox`
* `--disable-infobars`
* `--disable-dev-shm-usage`

### 4.2 Tarayıcı Parametreleri

* `userAgent`
* `viewport` (width, height, deviceScaleFactor)
* `locale`
* `timezoneId`
* `language`
* `plugins`
* `webglVendor`
* `webglRenderer`

### 4.3 Örnek Playwright Yapılandırması

```js
const context = await browser.newContext({
  userAgent: "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
  locale: "tr-TR",
  timezoneId: "Europe/Istanbul",
  viewport: { width: 1366, height: 768 },
});
```

### 4.4 Örnek Selenium Yapılandırması

```python
from selenium import webdriver
from selenium.webdriver.chrome.options import Options

options = Options()
options.add_argument("--disable-blink-features=AutomationControlled")
options.add_argument("--no-sandbox")
options.add_argument("--disable-infobars")

driver = webdriver.Chrome(options=options)
```

---

## 5. Güvenlik Açısından Kritik Noktalar

Stealth automation teknikleri, hem teknik hem de hukuki riskler taşır.

### 5.1 Hukuki ve Etik Riskler

* Birçok web sitesinin Kullanım Şartları (ToS) ihlal edilebilir
* CAPTCHA ve bot tespit sistemlerini aşmak bazı ülkelerde suç teşkil edebilir
* Yetkisiz scraping veri ihlallerine yol açabilir

### 5.2 Teknik Riskler

* Eksik fingerprint maskesi account ban riskini artırır
* IP reputation bozulabilir
* Proxy leak’leri gerçek IP’nin açığa çıkmasına neden olabilir
* WebGL ve canvas fingerprint tutarsızlıkları bot olarak işaretlenmeye yol açar

### 5.3 Güvenli Kullanım Önerileri

Stealth automation yalnızca:

* Test
* QA
* Akademik araştırma
* Güvenlik simülasyonu

amaçlı kullanılmalıdır.

* Rate-limit ve davranış profili uygulanmalıdır
* Proxy rotation ve IP reputation kontrolü yapılmalıdır

---

## 6. Proje Entegrasyonu ve Uygulama Adımları

Bu repo’yu kendi çalışmana entegre etmek için önerilen adımlar:

1. GitHub reposunu fork et
2. Local ortama clone et
3. Gerekli bağımlılıkları yükle
4. Headless ve headed modları karşılaştır
5. Fingerprint maskelerini test et
6. Davranış simülasyonlarını ekle
7. Bot detection test sitelerinde doğrula
8. Log ve hata ayıklama mekanizması ekle

---

## Kaynaklar

* [https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation](https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation)
* [https://github.com/berstend/puppeteer-extra](https://github.com/berstend/puppeteer-extra)
* [https://github.com/ultrafunkamsterdam/undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)
* [https://github.com/AtuboDad/playwright-stealth](https://github.com/AtuboDad/playwright-stealth)
* [https://playwright.dev](https://playwright.dev)
* [https://www.selenium.dev](https://www.selenium.dev)
* [https://fingerprintjs.com](https://fingerprintjs.com)
