# KluxLock

KluxLock, Android cihazlarda uygulamalarınızı ek bir güvenlik katmanıyla korumak için geliştirilmiş açık kaynaklı bir uygulama kilitleme projesidir. Biyometrik doğrulama, PIN koruması ve farklı uygulama algılama yöntemleriyle kişisel verilerinizi daha güvenli tutmayı hedefler.

## Neler Sunar?

- İstediğiniz uygulamaları tek tek kilitleme
- Biyometrik doğrulama desteği
- PIN ile güvenli giriş
- Erişilebilirlik, kullanım istatistikleri ve Shizuku tabanlı farklı algılama yöntemleri
- Uygulama kaldırmayı zorlaştıran ek koruma seçenekleri
- Arka planda çalışmayı iyileştirmek için pil optimizasyonu yönlendirmeleri
- Modern Jetpack Compose tabanlı arayüz

## Kimler İçin Uygun?

KluxLock özellikle şu kullanım senaryoları için uygundur:

- Mesajlaşma, banka, galeri veya not uygulamalarını korumak isteyen kullanıcılar
- Cihazını başkalarıyla paylaşan ama bazı uygulamalarını gizli tutmak isteyenler
- Açık kaynak, reklamsız ve daha şeffaf bir uygulama kilidi çözümü arayanlar

## Teknik Özet

Proje Android ve Kotlin tabanlıdır. Arayüz tarafında Jetpack Compose kullanılır. Uygulama, farklı cihaz ve kullanım senaryolarına uyum sağlamak için birden fazla arka plan çalışma yaklaşımını destekler.

Öne çıkan yapılar:

- `app`: Ana Android uygulaması
- `appintro`: İlk kurulum ve tanıtım akışı
- `patternlock`: Desen kilidi bileşenleri
- `hidden-api`: Gelişmiş sistem entegrasyonları için yardımcı katman

## Gereksinimler

- Android Studio
- JDK 17
- Android SDK 36
- Minimum Android sürümü: 8.0 (API 26)

## Kurulum ve Çalıştırma

Projeyi yerelde çalıştırmak için:

```bash
git clone <repo-url>
cd KluxLock
./gradlew assembleDebug
```

Android Studio ile açıp doğrudan `app` modülünü de çalıştırabilirsiniz.

## İzinler Hakkında

KluxLock, çalışma mantığı gereği bazı özel izinlere ihtiyaç duyar. Bunlar kullanılan moda göre değişebilir:

- Erişilebilirlik izni
- Kullanım istatistikleri erişimi
- Diğer uygulamaların üzerinde gösterme izni
- Bildirim izni
- Pil optimizasyonundan muaf tutma
- İsteğe bağlı olarak Shizuku erişimi

Bu izinler, kilit ekranını doğru zamanda göstermek ve korumayı arka planda sürdürebilmek için kullanılır.

## Projenin Amacı

Bu proje, kullanıcı gizliliğini merkeze alan, modern Android sürümleriyle uyumlu ve geliştirilebilir bir uygulama kilidi altyapısı sunmayı amaçlar. Hem son kullanıcılar hem de Android güvenlik ve gizlilik araçları üzerinde çalışan geliştiriciler için iyi bir temel oluşturur.

## Not

Shizuku tabanlı özellikler gelişmiş kullanıcılar içindir. Bu moddan tam verim almak için ek kurulum adımları ve ADB tarafında yapılandırma gerekebilir.

## Forked/Skidded from
https://github.com/aload0/AppLock

Proje sadece türkcelestirildi geri kalan hersey ayni.