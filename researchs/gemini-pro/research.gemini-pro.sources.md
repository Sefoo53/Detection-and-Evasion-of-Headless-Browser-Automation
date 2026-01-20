# research.gemini-pro.sources.md

## Detection and Evasion of Headless Browser Automation  
**Gemini Pro Kaynak Derleme Dosyası**

Bu dosya, headless browser automation tespiti ve kaçınma teknikleri üzerine yapılan ileri seviye teknik araştırmada kullanılan ana kaynakları içermektedir.

---

## 1. Resmî Dokümantasyonlar

1. Puppeteer Documentation  
   - https://pptr.dev  
   - Konular:  
     - Chrome DevTools Protocol  
     - evaluateOnNewDocument  
     - Headless mode  
     - User-Agent & Client Hints  

2. Playwright Documentation  
   - https://playwright.dev  
   - Konular:  
     - Browser context spoofing  
     - Permissions API  
     - Stealth yapılandırma  

3. Selenium Documentation  
   - https://www.selenium.dev  
   - Konular:  
     - WebDriver izleri  
     - ChromeOptions  
     - undetected-chromedriver  

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

## 3. Teknik Makaleler ve Bloglar

1. Bot Detection Techniques on the Web  
   - Konu: Bot tespit mekanizmaları  
   - İçerik: Fingerprinting, davranışsal analiz, ML tabanlı bot tespiti  

2. TLS Fingerprinting (JA3/JA4) Explained  
   - Konu: TLS fingerprinting  
   - İçerik: JA3/JA4 hash mekanizmaları  

3. How Websites Detect Headless Browsers  
   - Konu: Headless tarayıcı tespit yöntemleri  
   - İçerik: navigator.webdriver, fingerprinting  

---

## 4. JavaScript API Referansları

1. navigator.webdriver  
   - Açıklama: Tarayıcının otomasyon tarafından kontrol edilip edilmediğini belirtir.

2. navigator.userAgentData  
   - Açıklama: Client Hints API

3. CanvasRenderingContext2D  
   - Açıklama: Canvas fingerprinting

4. WebGLRenderingContext  
   - Açıklama: GPU vendor ve renderer bilgisi

5. AudioContext  
   - Açıklama: Audio fingerprinting

---

## 5. Güvenlik ve Etik Notlar

- Bu kaynaklar yalnızca:
  - Güvenlik araştırması  
  - QA otomasyonu  
  - Akademik çalışmalar  

  için kullanılmalıdır.

- Kötüye kullanım etik ve hukuki sorunlara yol açabilir.

---

**Dosya:** `research.gemini-pro.sources.md`  
**Amaç:** Headless browser detection & evasion araştırması için ileri seviye referans kaynak havuzu
