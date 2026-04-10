# Space Shooter Game

[![Oyun Görseli/Demo](https://img.shields.io/badge/Oyun-HTML5%20Canvas-blue.svg)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](#)

Tamamen **HTML5 Canvas** ve **Vanilla JavaScript** kullanılarak geliştirilmiş, retro tarzı aksiyon dolu bir uzay nişancı (Space Shooter) oyunudur. Tarayıcı üzerinde hiçbir ek kütüphane gerektirmeden çalışır.

## 📌 Özellikler

*   **Platform Bağımsız:** Tamamen responsive (duyarlı) yapısı sayesinde masaüstü ve mobil ekranlara kendini otomatik uydurur.
*   **Gelişmiş Düşmanlar ve Dalgalar (Waves):** Farklı rotalara sahip (düz, sinüs dalgası şeklinde, oyuncuya doğru dalan) düşman tipleri. Her 5 dalgada bir özel "Boss" savaşı başlar.
*   **Prosedürel Ses Sistemi:** Dışarıdan büyük MP3 / WAV dosyaları yüklemek yerine, tüm patlama, lazer, ateş, hasar ve boss sesleri **Web Audio API** kullanılarak anlık (procedural) olarak sentezlenir.
*   **Özel Efektler (VFX):** Anlık ekran titremesi (screen shake), çeşitli boyutta parçalanabilen meteorlar, dinamik yıldız tarlası (starfield) arkaplanı ve patlama parçaçıkları.
*   **Güçlendirmeler (Power-Ups):** Savaşırken üç farklı özel yeteneği düşürebilirsiniz:
    *   ⚡ **Seri Atış (Rapid Fire)**: Atış hızını maksimize eder.
    *   ★ **Üçlü Atış (Triple Shot)**: Aynı anda 3 yöne ateş etmenizi sağlar.
    *   🛡️ **Kalkan (Shield)**: Belirli bir hasar limitine kadar geminizi korur (HUD üzerinde canı görünür).
*   **Skor Kaydı:** En yüksek skorunuz (High Score) tarayıcınızın `localStorage`'ına kaydedilir ve sayfa yenilense de silinmez.

## 🎮 Kontroller

Oyun, hem klavye algılayıcısını hem de mobilde sanal butonları destekler.

### Masaüstü (Klavye)
*   **Hareket:** Yön okları (`←`, `↑`, `→`, `↓`)
*   **Ateş Etme:** `Boşluk (Space)` veya `Enter` (Ayıca oyunu başlatır veya yeniden başlatır)
*   **Duraklat (Pause):** `Esc`

### Mobil (Dokunmatik Ekran)
*   **Hareket:** Ekranın sol yarısında beliren Sanal Joystick.
*   **Ateş Etme:** Ekranın sağ alt kısmındaki "FIRE" ikalasına dokunarak/basılı tutarak.
*   *Menüleri geçmek için ekrana dokunun.*

## 🛠️ Kurulum ve Çalıştırma

Oyun tamamen istemci tarafında (client-side) çalışır. Herhangi bir sunucu kurumuna (Node.js, Python vb.) ihtiyacınız yoktur.

1.  Bu projeyi diskinize indirin (veyahut klonlayın).
2.  Projenin aynı dizininde `index.html` dosyası ve oyun resimlerini barındıran `PNG` klasörü bulunmalıdır.
3.  `index.html` dosyasına çift tıklayıp modern bir web tarayıcısında (Chrome, Firefox, Edge, Safari vb.) açmanız yeterlidir.

## 🧰 Kullanılan Teknolojiler

*   **HTML:** `<canvas>` elementi şablonu.
*   **CSS:** Tarayıcı sıfırlama (reset) ve temel canvas konumlandırma optimizasyonu.
*   **JavaScript (ES6):**
    *   Oyun döngüsü (Game Loop via `requestAnimationFrame`)
    *   Entity-Component mantığına benzer Sınıf (Class) bazlı obje yönetimi
    *   Basit Dörtgen Çarpışma Tespitleri (AABB Collision)
*   **Web Audio API:** Ses sentezleme.

---
*İyi Eğlenceler!*
