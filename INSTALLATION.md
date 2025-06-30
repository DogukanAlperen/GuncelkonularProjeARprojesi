# 🔧 INSTALLATION.md - Kurulum Rehberi

Bu döküman, AR Racing Game projesini sorunsuz bir şekilde çalıştırmak isteyen kullanıcılar ve geliştiriciler için detaylı kurulum talimatlarını içerir.

---

## 📋 Gereksinimler

| Yazılım | Sürüm |
|--------|-------|
| Unity | 2021.3.x LTS veya 2022.x URP destekli |
| Android Build Support | Yüklü olmalı |
| AR Foundation | 4.x veya üzeri |
| ARCore XR Plugin | 4.x veya üzeri |
| XR Plugin Management | 4.x veya üzeri |
| Git | (Opsiyonel) Repository'yi klonlamak için |

---

## 🧰 Bağımlılıklar

Unity Package Manager üzerinden aşağıdaki bağımlılıkları yükleyin:

- **AR Foundation** → `Unity Registry > AR Foundation`
- **ARCore XR Plugin**
- **XR Plugin Management**
- **URP (Universal Render Pipeline)`**

---

## 🚀 Kurulum Adımları

1. **Unity Hub ile Projeyi Aç**
    - Unity Hub üzerinden `Open` diyerek bu projeyi açın.
    - Gerekirse uygun `Unity 2021.3.x` veya `2022.x` sürümünü kurun.

2. **Proje Ayarlarını Kontrol Et**
    - `Edit > Project Settings > XR Plugin Management`
        - Android için ARCore aktif olmalı.
    - `Graphics` ayarlarında URP aktif olmalı.

3. **Build Ayarları**
    - `File > Build Settings > Android`
    - `Scenes in Build` içine `MainGameAR_AR_Foundation.unity` sahnesini ekle
    - `Player Settings > XR Settings` altında:
        - ARCore destekleniyor işaretli olmalı
        - Minimum API Level: Android 7.0 (API 24) veya üzeri

---

## 📱 Uygulamanın Derlenmesi (Build)

- Cihazınızı USB ile bağlayın ve `Developer Mode` aktif olsun.
- Unity'den `Build and Run` diyerek cihazınıza yükleyin.

---

## 🧯 Troubleshooting

| Sorun | Çözüm |
|------|--------|
| Kamera çalışmıyor | ARCore destekli cihaz kullanın. Android izinlerini kontrol edin. |
| Build başarısız | Android Build Support eksik olabilir. Unity Hub’dan ekleyin. |
| AR yüzey algılanmıyor | Işıklı ortamda deneyin, yüzey düz ve belirgin olmalı. |

---

## 📄 Notlar

- AR destekli cihaz gereklidir.
- iOS için ARKit desteği ile ayrı bir yapı gerekir (şu an Android test edilmiştir).
