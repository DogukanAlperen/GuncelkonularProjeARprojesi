🧠 ARRacingGame: Artırılmış Gerçeklik Tabanlı Mobil Yarış Oyunu
🎮 Oyun Konsepti
ARRacingGame, Unity ve AR Foundation kullanılarak geliştirilen, oyuncunun fiziksel dünyasını dijital yarış pistine dönüştüren artırılmış gerçeklik (AR) tabanlı bir mobil yarış oyunudur.


|Demos||
|---|---|
|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_1.gif" width="300">|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_2.gif" width="300">|
|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_3.gif" width="300">|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_4.gif" width="300">|

Oyuncu, gerçek yüzeyde oluşturulan pistte aracını sürer, engelleri aşar ve görev tabanlı ilerlemeyle deneyimini zenginleştirir. Proje özellikle eğitsel AR uygulamaları, çocuklara yönelik etkileşimli oyunlar, ve AR geliştirici örnekleri için tasarlanmıştır.

🧩 Oyun Özellikleri
🚗 Oyun Başlangıcı & AR Yerleşimi
Oyuncu, telefonu fiziksel yüzeye tutar ve yarış pistini artırılmış gerçeklik ortamında yerleştirir.

Pist zemine sabitlenir ve fizik motoru aktif hale gelir.

AR destekli eğitim ekranı oyuncuyu yönlendirir.

🕹️ Kontroller
Joystick veya cihazın ivmeölçer sensörü (tilt) ile aracın yönlendirilmesi sağlanır.

Aracın ivmesi ve yönü fizik motoru ile yönetilir (Rigidbody, WheelCollider gibi).

🎯 Oynanış Dinamikleri
Oyuncu gerçek dünya üzerinde sanal pistte ilerler.

Pistte checkpoint’ler, engeller, hızlandırıcılar ve yön değiştirici bölgeler yer alır.

Oyuncu, hız kontrolü ve manevra yaparak pist dışına çıkmadan ilerlemelidir.

🧠 Görev ve Gelişim Mekanikleri
Not: Bu bölüm videoda vurgulanabilir – “Eğitsel genişletme opsiyonu olarak düşünülmüştür.”

Pist üzerinde görev istasyonları tanımlanabilir (checkpoint ile eşleştirilmiş).

Örnek görev: "Belirli sürede bitiş çizgisine ulaş", "X adet hızlandırıcı topla".

Oyunun bu bölümü kolayca genişletilebilir (ScriptableObject ile görev tanımı yapılabilir).

💡 Kullanılan Modüller & Teknolojiler
Modül	Açıklama
AR Foundation	AR oturumu başlatır, çevreyi algılar ve yüzey yerleştirme sağlar.
ARCore XR Plugin	Android cihazlarda AR Foundation ile entegrasyonu sağlar.
XR Plugin Management	ARCore ve diğer AR altyapılarının cihaz bazlı kontrolünü sağlar.
URP (Universal Render Pipeline)	Hafif, mobil uyumlu ve performans odaklı render altyapısı.
Physics & Rigidbody Sistemi	Araç sürüş fiziği, hızlanma ve yönlendirme kontrolleri için.
UI Sistemleri	Joystick, görev panelleri ve görsel geri bildirimler için.
Shader Optimization	AR görüntüsü için ARCameraBackground ve URP uyumlu materyaller.

🛡️ Güvenlik & Uyum
AR kamera erişimi için Android manifest’e özel izinler eklenmiştir.

Uygulama, mobil cihazlarda performans dostu olacak şekilde optimize edilmiştir.

AR kurulumu başlamadan önce kullanıcıya alan güvenliği uyarısı verilebilir (eklenebilir modül).

📈 Geliştirme Notları
Unity Sürümü: 2021.3.x LTS veya 2022+ URP destekli

Platform Desteği: Android (ARCore), iOS (ARKit destekli sürüm geliştirilebilir)

Sahne Dosyası: MainGameAR_AR_Foundation.unity

Yapılandırma: Assets/Scenes/, Assets/Scripts/, Assets/Art/, Assets/AR/
