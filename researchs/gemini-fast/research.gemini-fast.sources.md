# research.gemini-fast.sources.md

## Detection and Evasion of Headless Browser Automation  
**Kaynak Derleme Dosyası**

Bu dosya, headless browser automation tespiti ve kaçınma teknikleri üzerine yapılan teknik araştırmada kullanılan ana kaynakları, makaleleri, GitHub projelerini ve referans dokümanları içermektedir.

---

## 1. Akademik ve Teknik Makaleler

1. *Bot Detection Techniques on the Web*  
   - Konu: Web tabanlı bot tespit mekanizmaları  
   - İçerik: Fingerprinting, davranış analizi, JavaScript API kontrolleri  
   - Anahtar Kavramlar: Canvas fingerprinting, WebGL, timing analysis  

2. *Fingerprinting Techniques for Web Browsers*  
   - Konu: Tarayıcı parmak izi yöntemleri  
   - İçerik: Plugin listesi, font tespiti, ekran çözünürlüğü, GPU bilgileri  

3. *Behavior-Based Bot Detection*  
   - Konu: İnsan davranışına dayalı bot tespiti  
   - İçerik: Mouse hareketleri, scroll pattern, form doldurma süreleri  

---

## 2. Resmî Dokümantasyonlar

1. Puppeteer Documentation  
   - https://pptr.dev  
   - Konular:  
     - Headless mode  
     - User-Agent override  
     - evaluateOnNewDocument  
     - Browser launch flags  

2. Playwright Documentation  
   - https://playwright.dev  
   - Konular:  
     - Stealth configuration  
     - Browser context spoofing  
     - Permissions API  

3. Selenium Documentation  
   - https://www.selenium.dev  
   - Konular:  
     - WebDriver özellikleri  
     - `navigator.webdriver` davranışı  
     - ChromeOptions  

---

## 3. Açık Kaynak Projeler

1. Detection-and-Evasion-of-Headless-Browser-Automation  
   - https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation  
   - Açıklama:  
     Headless tarayıcıların nasıl tespit edildiğini ve bu tespitlerden kaçınma yöntemlerini gösteren referans proje.

2. puppeteer-extra-plugin-stealth  
   - https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-stealth  
   - Açıklama:  
     Puppeteer için stealth (gizlenme) eklentisi.  
     navigator.webdriver, WebGL, plugins ve permissions spoofing içerir.

3. playwright-stealth  
   - https://github.com/AtuboDad/playwright-stealth  
   - Açıklama:  
     Playwright için stealth patch koleksiyonu.

4. undetected-chromedriver  
   - https://github.com/ultrafunkamsterdam/undetected-chromedriver  
   - Açıklama:  
     Selenium tabanlı bot tespit kaçınma sürücüsü.

---

## 4. Blog Yazıları ve Teknik İncelemeler

1. *How Websites Detect Headless Browsers*  
   - Konu: Headless tarayıcı tespit teknikleri  
   - İçerik:  
     - navigator.webdriver  
     - User-Agent analizi  
     - WebGL & Canvas fingerprinting  
     - Plugin ve font kontrolleri  

2. *Evading Bot Detection in Puppeteer*  
   - Konu: Puppeteer stealth yöntemleri  
   - İçerik:  
     - Blink feature flag kapatma  
     - evaluateOnNewDocument kullanımı  
     - Fingerprint spoofing  

3. *Modern Bot Detection Techniques*  
   - Konu: Güncel bot tespit stratejileri  
   - İçerik:  
     - Behavioral detection  
     - ML tabanlı analiz  
     - Device fingerprinting  

---

## 5. JavaScript API Referansları

1. navigator.webdriver  
   - Açıklama:  
     Tarayıcının otomasyon tarafından kontrol edilip edilmediğini belirtir.

2. navigator.languages  
   - Açıklama:  
     Kullanıcının tercih ettiği dilleri döndürür.

3. navigator.plugins  
   - Açıklama:  
     Yüklü tarayıcı plugin listesini verir.

4. CanvasRenderingContext2D  
   - Açıklama:  
     Canvas fingerprinting için kullanılır.

5. WebGLRenderingContext  
   - Açıklama:  
     GPU vendor ve renderer bilgisini verir.

---

## 6. Güvenlik ve Etik Notlar

- Bu kaynaklar yalnızca:
  - Güvenlik araştırması  
  - Bot tespit sistemlerini anlama  
  - Otomasyon testleri  
  - Akademik çalışmalar  

  için kullanılmalıdır.

- Kötüye kullanım (scraping abuse, fraud, rate-limit bypass) etik ve hukuki sorunlara yol açabilir.

---

## 7. Notlar

- Kaynaklar zamanla güncelliğini yitirebilir.  
- Yeni stealth teknikleri ve tespit yöntemleri düzenli olarak takip edilmelidir.  
- Bu dosya, ana README.md ve teknik raporlar için referans olarak tasarlanmıştır.

---

**Dosya:** `research.gemini-fast.sources.md`  
**Amaç:** Headless browser detection & evasion araştırması için referans kaynak havuzu
