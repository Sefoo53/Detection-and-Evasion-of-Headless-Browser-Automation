# research.chatgpt.sources.md

## Detection and Evasion of Headless Browser Automation  
**ChatGPT Kaynak Derleme Dosyası**

Bu dosya, headless browser automation tespiti ve kaçınma teknikleri üzerine yapılan teknik araştırmada kullanılan ana kaynakları içermektedir.

---

## 1. Resmî Dokümantasyonlar

1. Puppeteer Documentation  
   - https://pptr.dev  
   - Konular:  
     - Headless mode  
     - User-Agent override  
     - evaluateOnNewDocument  

2. Playwright Documentation  
   - https://playwright.dev  
   - Konular:  
     - Browser context spoofing  
     - Permissions API  
     - Stealth yapılandırma  

3. Selenium Documentation  
   - https://www.selenium.dev  
   - Konular:  
     - WebDriver özellikleri  
     - ChromeOptions  
     - navigator.webdriver  

---

## 2. Açık Kaynak Projeler

1. Detection-and-Evasion-of-Headless-Browser-Automation  
   - https://github.com/Sefoo53/Detection-and-Evasion-of-Headless-Browser-Automation  

2. puppeteer-extra-plugin-stealth  
   - https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-stealth  

3. playwright-stealth  
   - https://github.com/AtuboDad/playwright-stealth  

4. undetected-chromedriver  
   - https://github.com/ultrafunkamsterdam/undetected-chromedriver  

---

## 3. Teknik Bloglar ve İncelemeler

1. How Websites Detect Headless Browsers  
   - Konu: Headless tarayıcı tespit yöntemleri  
   - İçerik: navigator.webdriver, fingerprinting, davranışsal analiz  

2. Evading Bot Detection in Puppeteer  
   - Konu: Puppeteer stealth teknikleri  
   - İçerik: Blink feature flags, fingerprint spoofing  

3. Modern Bot Detection Techniques  
   - Konu: Güncel bot tespit stratejileri  
   - İçerik: ML tabanlı bot tespiti, device fingerprinting  

---

## 4. JavaScript API Referansları

1. navigator.webdriver  
   - Açıklama: Tarayıcının otomasyon tarafından kontrol edilip edilmediğini belirtir.

2. navigator.languages  
   - Açıklama: Kullanıcının tercih ettiği dilleri döndürür.

3. navigator.plugins  
   - Açıklama: Yüklü tarayıcı plugin listesini verir.

4. CanvasRenderingContext2D  
   - Açıklama: Canvas fingerprinting için kullanılır.

5. WebGLRenderingContext  
   - Açıklama: GPU vendor ve renderer bilgisini verir.

---

## 5. Güvenlik ve Etik Notlar

- Bu kaynaklar yalnızca:
  - Güvenlik araştırması  
  - QA otomasyonu  
  - Akademik çalışmalar  

  için kullanılmalıdır.

- Kötüye kullanım (scraping abuse, fraud, rate-limit bypass) etik ve hukuki sorunlara yol açabilir.

---

**Dosya:** `research.chatgpt.sources.md`  
**Amaç:** Headless browser detection & evasion araştırması için referans kaynak havuzu
