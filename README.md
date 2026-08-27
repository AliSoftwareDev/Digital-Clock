  # Digital Clock Application

Ekran üzerinde anlık zamanı, tarihi ve gün bilgisini canlı olarak güncelleyen, minimalist ve modern arayüz tasarımına sahip **Vanilla JavaScript** dijital saat uygulaması.

---

## 📸 Ekran Görüntüsü

<img width="1280" height="720" alt="Screen Recording 2026-08-27 at 10 51 45 47 PM" src="https://github.com/user-attachments/assets/35bb9e7b-300b-4d20-9b64-2bd715b1d598" />


---

## 🚀 Özellikler

* **Gerçek Zamanlı Senkronizasyon:** JavaScript `setInterval` mekanizması ile saat, dakika ve saniye verilerinin her 1000ms (1 saniye) aralığında milisaniyelik sapma olmadan güncellenmesi.
* **Format Düzenleme (Zero Padding):** Tek haneli sayıların (örn: 9) önüne dinamik olarak sıfır eklenerek (`09`) saat formatının bozulmasının önlenmesi (`padStart` kullanımı).
* **Tarih ve Gün Bilgisi:** Sistem zamanına bağlı olarak güncel gün, ay ve yıl bilgisinin yerelleştirilmiş formatta ekrana basılması.
* **Responsive & Tipografik Tasarım:** Farklı ekran çözünürlüklerinde okunabilirliği koruyan, dijital saat fontları veya monospaced yazı tipleriyle desteklenmiş responsive layout.

---

## 🛠️ Teknolojik Mimari

* **HTML5:** Semantik zaman etiketleri (`<time>`) ve konteyner yapısı.
* **CSS3:** 
  * `flexbox` / `grid` ile ekranın tam ortasına hizalama (center layout)
  * CSS değişkenleri ve karanlık tema (Dark Mode) uyumu
  * Metin gölgeleri (`text-shadow`) ile dijital ekran efekti
* **Vanilla JavaScript (ES6+):** 
  * `Date` nesnesi metotları (`getHours`, `getMinutes`, `getSeconds`)
  * `String.prototype.padStart()` ile formatlama
  * Zamanlayıcı fonksiyonlar (`setInterval`)

---

## 📂 Proje Dosya Yapısı

```text
digital-clock/
│
├── assets/
│   └── preview.png       # README ekran görüntüsü
├── index.html            # Saat gösterge alanları ve iskelet
├── clock.css             # Tipografi, renkler ve ekran hizalaması
├── clock.js             # Date objesi işleme ve zamanlayıcı döngüsü
└── README.md             # Proje dokümantasyonu
