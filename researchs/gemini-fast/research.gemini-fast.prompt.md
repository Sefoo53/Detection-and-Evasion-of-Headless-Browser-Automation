# research.gemini-fast.prompt.md

## Detection and Evasion of Headless Browser Automation

**Araştırma Prompt Dosyası**

Bu dosya, Gemini Fast modeli kullanılarak yapılan teknik araştırmada modele verilen ana promptları ve görev tanımlarını içerir.

---

## 🎯 Ana Araştırma Amacı

Headless browser automation (Puppeteer, Playwright, Selenium vb.) tespit mekanizmalarını ve bu mekanizmalardan kaçınma (evasion) tekniklerini teknik düzeyde analiz etmek.

---

## 🧠 Kullanılan Ana Prompt

```
Detection-and-Evasion-of-Headless-Browser-Automation konusu hakkında
detaylı bir teknik araştırma yap.

Bu teknolojinin temel çalışma prensiplerini açıkla.

Web sitelerinin headless tarayıcıları nasıl tespit ettiğini teknik olarak anlat.

Kullanılan başlıca detection tekniklerini listele:

- navigator.webdriver
- User-Agent analizi
- WebGL & Canvas fingerprinting
- Plugin ve font kontrolleri
- Davranışsal analiz (mouse, scroll, timing)

Bu tespit yöntemlerinden kaçınma (evasion) tekniklerini açıkla.

Puppeteer, Playwright ve Selenium için örnek kodlar ver.

Güvenlik ve etik açıdan riskleri belirt.

En iyi uygulamaları (best practices) çıkar.

Açık kaynak projeleri ve rakipleri listele.

Sonuç ve öneriler bölümü oluştur.

Cevapları teknik seviyede, başlıklandırılmış ve Markdown formatında üret.
```

---

## 🧩 Ek Alt Promptlar

### 1. Detection Teknikleri Derinleştirme

Web sitelerinin headless browser'ları tespit etmek için
kullandığı modern teknikleri teknik detaylarıyla açıkla.

* JavaScript API kontrolleri
* Fingerprinting yöntemleri
* Behavioral detection
* ML tabanlı bot tespiti

---

### 2. Evasion Teknikleri Derinleştirme

Headless tarayıcıların bot olarak algılanmaması için
kullanılan modern evasion tekniklerini açıkla.

* navigator.webdriver gizleme
* User-Agent spoofing
* WebGL & Canvas masking
* İnsan davranışı simülasyonu
* Proxy ve IP rotasyonu

---

### 3. Kod Üretim Promptu

Puppeteer ve Playwright kullanarak
bot tespitinden kaçınmaya yönelik
örnek JavaScript kodları üret.

* evaluateOnNewDocument kullanımı
* Blink feature flag kapatma
* Gerçekçi fingerprint ayarları

---

## 📌 Prompt Notları

* Teknik doğruluk önceliklidir.
* Akademik dil tercih edilmiştir.
* Kod örnekleri yorum satırlarıyla açıklanmalıdır.
* Etik ve hukuki uyarılar mutlaka eklenmelidir.

---

## 🗂 Dosya Amacı

Bu dosya:

* Araştırma sürecinde kullanılan promptların arşivi
* Sonuç dosyasının (`research.gemini-fast.result.md`) nasıl üretildiğinin kaydı
* Yeniden üretilebilirlik (reproducibility) için referans

amacıyla hazırlanmıştır.
