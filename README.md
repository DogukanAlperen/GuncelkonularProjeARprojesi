# 🧠 ARRacingGame: Artırılmış Gerçeklik Tabanlı Mobil Yarış Oyunu

Unity ve AR Foundation kullanılarak geliştirilen bu mobil oyun, oyuncunun fiziksel ortamını dijital yarış pistine dönüştüren bir artırılmış gerçeklik (AR) deneyimi sunar.

🎥 [Tanıtım Videosu (YouTube)](https://youtu.be/kp92tWjbj8I)

---

## 🎯 Projenin Amacı ve Hedef Kitlesi

Bu proje;
- AR tabanlı oyun geliştirme süreçlerini öğrenmek isteyen geliştiricilere,
- Eğitsel oyun içeriği sunmak isteyen eğitmenlere,
- AR destekli mobil oyunlara ilgi duyan genel oyuncu kitlesine hitap etmektedir.

---

## 💻 Kullanılan Teknolojiler ve Framework’ler

| Teknoloji | Açıklama |
|----------|----------|
| Unity (2021.3.x veya 2022.x URP) | Geliştirme ortamı |
| AR Foundation | AR oturumu başlatma, yüzey algılama |
| ARCore XR Plugin | Android cihazlarla entegrasyon |
| XR Plugin Management | ARCore kontrolü |
| URP | Performans dostu render altyapısı |
| Rigidbody & WheelCollider | Araç fiziği |
| UI System | Joystick, butonlar, görev panelleri |
| Shader Optimization | AR Camera Background & URP uyumlu shader'lar |

---

## ⚙️ Kurulum Rehberi

🔧 Detaylı kurulum için [INSTALLATION.md](INSTALLATION.md) dosyasına bakınız.

### Kısa Kurulum Adımları:

1. Unity Hub ile projeyi açın (2021.3.x veya 2022.x URP).
2. Gerekli paketleri yükleyin:
   - AR Foundation
   - ARCore XR Plugin
   - XR Plugin Management
3. `Build Settings > Android` seçin.
4. `MainGameAR_AR_Foundation.unity` sahnesini ekleyin.
5. `Build and Run` diyerek cihazda çalıştırın.

---

## 🚀 Kullanım Talimatları

📘 Detaylı kullanım için [USER_MANUAL.md](USER_MANUAL.md) dosyasına göz atın.

### Temel Kullanım:

- Uygulamayı açın ve kamera izni verin.
- Telefonu düz bir yüzeye tutarak pist yerleşimini tamamlayın.
- Joystick veya tilt sensörü ile aracı yönetin.
- Checkpoint'leri geçin, görevleri tamamlayın.

---

## 🧩 Oyun Özellikleri

- 🛞 **AR Pist Yerleşimi**: Fiziksel yüzeye pist sabitlenir.
- 🎮 **Kontroller**: Joystick veya cihaz eğimi ile kontrol.
- 🔧 **Fizik Sistemi**: Rigidbody ve WheelCollider kullanımı.
- 🗺️ **Oynanış Dinamikleri**: Engeller, hızlandırıcılar, checkpoint’ler.
- 🎯 **Görev Sistemi**: ScriptableObject ile tanımlı görevler.
- 👨‍🏫 **Eğitsel Yapı**: Geliştirilebilir görev tabanlı yapı.

---

## 🧠 AR Özellikleri

| Özellik | Açıklama |
|--------|----------|
| AR Foundation | Oturum başlatma ve yüzey algılama |
| ARCore | Android cihazlarda AR destek sağlar |
| URP | Gerçekçi ve optimize görüntüleme |
| AR Kamera | Gerçek dünyayı ekran arkasına aktarır |
| Gerekli Donanım | ARCore destekli Android cihaz, kamera erişimi |

---

## 📸 Ekran Görüntüleri

> 📁 Görseller `screenshots/` klasöründe yer almalı

![Ana Menü](screenshots/menu.png)
![Pist Yerleşimi](screenshots/track.png)
![Yarış Başlangıcı](screenshots/start.png)
![Oynanış Ekranı](screenshots/gameplay.png)
![Görev Tamamlandı](screenshots/mission.png)

---

## 📱 APK Dosyası

📥 Uygulamanın APK dosyası `apk/` klasöründe yer almalıdır.

Alternatif olarak:
👉 [Google Drive Üzerinden İndir](https://drive.google.com/your-apk-link) *(örnek link)*

---

## 🛡️ Güvenlik ve Performans

- Kamera erişim izinleri `AndroidManifest.xml` içinde tanımlanmıştır.
- Cihaz uyumluluğu ARCore destekli Android cihazlardır.
- Uygulama düşük cihazlarda dahi stabil çalışacak şekilde optimize edilmiştir.
- Oyun öncesi fiziksel ortam güvenliği için uyarı gösterilebilir.

---

## 📈 Geliştirme Notları

- **Unity Sürümü:** 2021.3.x LTS / 2022.x URP
- **Platform Desteği:** Android (ARCore) – iOS uyumu geliştirilebilir
- **Ana Sahne:** `MainGameAR_AR_Foundation.unity`
- **Klasör Yapısı:** `src/Assets`, `src/Scripts`, `src/AR` şeklinde organize edilmiştir

---

## 📂 Proje Yapısı

