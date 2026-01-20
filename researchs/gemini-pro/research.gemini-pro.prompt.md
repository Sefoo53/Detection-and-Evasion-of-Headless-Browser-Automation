# research.gemini-pro.prompt.md

## Detection and Evasion of Headless Browser Automation  
**Gemini Pro Araştırma Prompt Dosyası**

Bu dosya, Gemini Pro modeli kullanılarak yapılan teknik araştırmada modele verilen ana promptları ve görev tanımlarını içerir.

---

## 🎯 Ana Araştırma Amacı

Headless browser automation (Puppeteer, Playwright, Selenium vb.) tespit mekanizmalarını ve bu mekanizmalardan kaçınma (evasion) tekniklerini ileri teknik seviyede analiz etmek.

---

## 🧠 Kullanılan Ana Prompt

Detection-and-Evasion-of-Headless-Browser-Automation konusu hakkında  
ileri seviye teknik bir araştırma yap.

Headless browser automation’ın temel çalışma prensiplerini açıkla.

Modern web sitelerinin bot tespiti için kullandığı yöntemleri teknik detaylarıyla anlat.

Gelişmiş detection tekniklerini listele:

- `navigator.webdriver`  
- User-Agent & Client Hints analizi  
- WebGL & Canvas fingerprinting  
- AudioContext fingerprinting  
- Plugin, font ve media device kontrolleri  
- Davranışsal analiz (mouse, scroll, timing)  
- ML tabanlı bot tespiti  

Gelişmiş evasion tekniklerini açıkla:

- Stealth patching  
- Fingerprint spoofing  
- İnsan davranışı simülasyonu  
- Proxy ve IP rotasyonu  
- TLS fingerprint masking  

Puppeteer, Playwright ve Selenium için gelişmiş örnek kodlar üret:

- `evaluateOnNewDocument` patch’leri  
- WebGL spoofing  
- Client Hints override  
- Davranış simülasyonu  

Güvenlik, etik ve hukuki riskleri belirt.

Best practices ve endüstri standartlarını çıkar.

Açık kaynak projeleri ve rakipleri karşılaştır.

Sonuç ve teknik öneriler bölümü oluştur.

Cevapları ileri teknik seviyede, başlıklandırılmış ve Markdown formatında üret.

---

## 🧩 Ek Alt Promptlar

### 1. Fingerprinting Derinleştirme

WebGL, Canvas, AudioContext ve Font fingerprinting  
yöntemlerini teknik detaylarıyla açıkla.

Bu fingerprint’lerin nasıl üretildiğini ve  
bot tespitinde nasıl kullanıldığını anlat.

---

### 2. TLS & Network Fingerprinting

TLS fingerprinting ve JA3/JA4 hash mekanizmalarının  
bot tespitinde nasıl kullanıldığını açıkla.

Bu tespitlerden kaçınma yöntemlerini belirt.

---

### 3. Kod Üretim Promptu

Puppeteer ve Playwright kullanarak  
gelişmiş stealth yapılandırması içeren  
örnek JavaScript kodları üret.

- `evaluateOnNewDocument` patch’leri  
- WebGL spoofing  
- Client Hints override  
- Davranış simülasyonu  

---

## 📌 Prompt Notları

- İleri teknik seviye dil kullanılmalıdır.  
- Kod örnekleri detaylı yorumlarla açıklanmalıdır.  
- Güvenlik, etik ve hukuki uyarılar mutlaka eklenmelidir.  
- Endüstri standartlarına referans verilmelidir.  

---

## 🗂 Dosya Amacı

Bu dosya:

- Gemini Pro ile yapılan araştırmada kullanılan promptların arşivi  
- Sonuç dosyasının (`research.gemini-pro.result.md`) nasıl üretildiğinin kaydı  
- Yeniden üretilebilirlik (reproducibility) için referans  

amacıyla hazırlanmıştır.
