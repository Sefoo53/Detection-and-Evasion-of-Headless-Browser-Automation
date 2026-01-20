# Detection and Evasion of Headless Browser Automation

Bu proje, modern web sitelerinin headless browser automation (Selenium, Puppeteer, Playwright) trafiğini nasıl tespit ettiğini ve bu tespit mekanizmalarına karşı hangi kaçınma (stealth) tekniklerinin uygulanabildiğini inceleyen deneysel bir çalışmadır.

Amaç; bot tespit sistemlerinin kullandığı fingerprint ve davranış tabanlı sinyalleri analiz etmek, bu sinyallerin nasıl maskelebileceğini göstermek ve güvenlik araştırmaları için referans bir kaynak oluşturmaktır.

---

## 🚀 Projenin Amacı

* Headless tarayıcıların tespit edilme nedenlerini analiz etmek
* Yaygın bot tespit sinyallerini sınıflandırmak
* Fingerprint tabanlı kontrolleri incelemek
* Davranış simülasyonu tekniklerini göstermek
* Stealth automation yaklaşımlarını karşılaştırmak

Bu repo, gerçek dünya bot tespit sistemlerinin (Akamai, PerimeterX, FingerprintJS vb.) kullandığı temel mantığı anlamaya yöneliktir.

---

## 🔍 Kapsam

Projede aşağıdaki alanlar ele alınmaktadır:

### Tespit Sinyalleri

* `navigator.webdriver` kontrolü
* Headless Chrome User-Agent paterni
* Plugin ve font eksiklikleri
* Canvas ve Audio fingerprint anomalileri
* WebGL vendor / renderer tutarsızlıkları
* Mouse / scroll davranışı eksikliği
* Timing pattern farklılıkları
* Proxy ve IP reputation

### Kaçınma (Evasion) Teknikleri

* `navigator.webdriver` override
* Headless flag’lerinin kapatılması
* Gerçekçi User-Agent ve viewport ayarları
* Plugin ve font enjeksiyonu
* Canvas ve WebGL fingerprint spoofing
* İnsan benzeri mouse ve scroll simülasyonu
* Locale, timezone ve dil eşitlemesi

---

## 🛠️ Kullanılan Teknolojiler

* Playwright
* Puppeteer
* Selenium
* JavaScript / Python
* Chrome DevTools Protocol

---

## ⚙️ Kurulum

```bash
git clone https://github.com/your-username/Detection-and-Evasion-of-Headless-Browser-Automation.git
cd Detection-and-Evasion-of-Headless-Browser-Automation
npm install
# veya
pip install -r requirements.txt
```

---

## ▶️ Kullanım

### Playwright Örneği

```js
const { chromium } = require("playwright");

const browser = await chromium.launch({ headless: false });
const context = await browser.newContext({
  userAgent: "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
  locale: "tr-TR",
  timezoneId: "Europe/Istanbul",
  viewport: { width: 1366, height: 768 },
});

const page = await context.newPage();
await page.goto("https://bot-detection-test-site.example");
```

---

## 🧪 Test Ortamı

Bu projedeki script’ler şu tip sitelerde test edilmiştir:

* FingerprintJS demo
* Bot detection test sayfaları
* Basit CAPTCHA içeren örnek siteler

---

## ⚠️ Hukuki ve Etik Uyarı

Bu proje **yalnızca** aşağıdaki amaçlarla kullanılmalıdır:

* Akademik araştırma
* QA ve otomasyon testleri
* Güvenlik simülasyonu
* Bot tespit sistemlerini anlamaya yönelik çalışmalar

Aşağıdaki durumlarda kullanımı **önerilmez**:

* Yetkisiz scraping
* CAPTCHA aşma
* Servis şartlarını (ToS) ihlal eden otomasyon
* Kötü niyetli bot faaliyetleri

Bu repoyu kullanan herkes, bulunduğu ülkenin hukuki düzenlemelerinden ve hedef sitelerin kullanım şartlarından sorumludur.

---

## 📌 Bilinen Limitasyonlar

* Tüm fingerprint sinyalleri %100 maskelemez
* Yeni tarayıcı sürümleriyle bazı teknikler bozulabilir
* Gelişmiş bot tespit sistemleri yine de tespit edebilir
* Proxy reputation kritik bir faktördür

---

## 🧩 Benzer Projeler

* puppeteer-extra-plugin-stealth
* undetected-chromedriver
* playwright-stealth
* Selenium Stealth

---

## 📚 Kaynaklar

* [https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation](https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation)
* [https://github.com/berstend/puppeteer-extra](https://github.com/berstend/puppeteer-extra)
* [https://github.com/ultrafunkamsterdam/undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)
* [https://github.com/AtuboDad/playwright-stealth](https://github.com/AtuboDad/playwright-stealth)
* [https://fingerprintjs.com](https://fingerprintjs.com)

---

## 🤝 Katkı

Pull request’ler ve issue’lar memnuniyetle karşılanır.

1. Fork et
2. Feature branch oluştur
3. Commit at
4. PR aç

---

## 📄 Lisans

Bu proje MIT lisansı altındadır.
