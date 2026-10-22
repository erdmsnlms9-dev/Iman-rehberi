# İman Rehberi — Android APK derleme paketi
Geliştirici imzası: ercan.ş

Bu paket, web uygulamasını Capacitor ile Android uygulamasına sarar ve GitHub Actions üzerinde debug APK derlemek için workflow içerir.

## Telefonda APK oluşturma
1. ZIP'i GitHub'a yeni bir repository olarak yükleyin (GitHub hesabı gerekir).
2. ZIP'in içeriğini repository'nin köküne çıkarılmış dosyalar olarak yükleyin; özellikle `.github/workflows/android.yml` dosyasının bulunduğundan emin olun.
3. Repository'de **Actions** sekmesini açın.
4. **Build Android APK** iş akışını seçip **Run workflow** düğmesine basın.
5. İşlem tamamlanınca workflow çalışmasının altındaki **Artifacts** bölümünden `iman-rehberi-debug-apk` dosyasını indirin.
6. İnen artifact ZIP'ini Dosyalar uygulamasında açın; içindeki `app-debug.apk` dosyasına dokunup yükleyin.
7. Android sorarsa yalnızca GitHub'dan indirdiğiniz kendi APK'nız için tarayıcı/Dosyalar uygulamasına "Bilinmeyen uygulamaları yükle" izni verin. Kurulumdan sonra bu izni kapatabilirsiniz.

## Önemli
- Bu bir debug APK'dır; kişisel kullanım/test içindir. Play Store yayını için imzalı release build ve gizlilik politikası gerekir.
- GitHub Actions derlemesi bu paket ortamında çalıştırılıp doğrulanmamıştır.
- Uygulama AlAdhan API'den namaz vakitleri çeker; internet gerekir.
- Günlük ayet/hadis içeriği sınırlı yerel seçkidir.
- Özel gün tarihleri örnek/tahminîdir, resmî Diyanet takvimiyle güncellenmelidir.
- Bildirimler uygulama açıkken tarayıcı/WebView ortamında sınırlıdır; Android uygulama kapalıyken kesin bildirim için native yerel bildirim entegrasyonu eklenmelidir.
