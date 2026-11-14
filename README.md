# CCTV Kayıt Süresi Hesaplayıcı

Kamera sayısı, çözünürlük, codec, FPS, sahne hareketi, günlük kayıt saati ve disk kapasitesine göre tahmini CCTV saklama süresini hesaplayan, tek sayfalık Türkçe web aracı.

## Özellikler

- 720p, 1080p, 1440p, 4 MP ve 4K çözünürlük seçenekleri
- H.264 ve H.265 için tahmini kamera bit hızı
- FPS ve sahne hareket yoğunluğuna göre ayarlama
- Gerçek bit hızını elle girme seçeneği
- Ses kaydı, günlük kayıt saati ve kullanılabilir disk alanı ayarı
- Tahmini saklama günü, günlük veri ve hedef süre için gereken disk hesabı
- Mobil uyumlu arayüz; harici kütüphane veya sunucu gerektirmez
- Tüm hesaplamalar tarayıcıda yapılır

## Çalıştırma

`index.html` dosyasını tarayıcıda açın. İnternet bağlantısı veya kurulum gerekmez.

## GitHub'da yayımlama

1. GitHub'da yeni bir **Public** depo oluşturun; örneğin `cctv-kayit-suresi-hesaplayici`.
2. Bu klasördeki `index.html` ve `README.md` dosyalarını deponun kök dizinine yükleyin.
3. Depoda **Settings → Pages** bölümünü açın.
4. **Build and deployment** altında **Deploy from a branch** seçin.
5. Branch olarak `main`, klasör olarak `/(root)` seçip **Save**'e basın.
6. GitHub Pages adresi aynı bölümde görünür.

## Hesaplama ve doğruluk

Otomatik bit hızı, seçilen çözünürlük için yaklaşık bir başlangıç değeriyle başlar ve codec, FPS ve hareket yoğunluğuna göre ölçeklenir. Kayıt cihazınızın gerçek bit hızı biliniyorsa elle girme seçeneğini kullanın.

Günlük veri yaklaşık olarak `toplam Mbps × kayıt saati × 0,45` formülüyle hesaplanır. Sonuç planlama tahminidir; gerçek değer kamera ayarlarına ve görüntü içeriğine göre değişir.

## Lisans

Bu ilk sürümde lisans dosyası eklenmemiştir. Yeniden kullanım koşullarını belirlemek isterseniz bir açık kaynak lisansı seçip depoya ekleyebilirsiniz.
