# 360° VR Video Player - Öğretmen Mesleği

Bu proje, `ogretmenVR.mp4` dosyasını 360 derece VR video player haline getirerek öğretmen mesleğine entegre eder.

## Özellikler

### 🎥 360° VR Video Player
- **Three.js** kullanarak 360 derece video oynatma
- **OrbitControls** ile fare ile etrafı keşfetme
- **Tam ekran** modu desteği
- **Oynat/Duraklat** kontrolü
- **Görünümü sıfırlama** özelliği

### 🎮 Kontroller
- **Fare sürükleme**: Etrafı keşfetmek için
- **Fare tekerleği**: Yakınlaştırma/uzaklaştırma
- **Kontrol butonları**: Oynat/Duraklat, Tam Ekran, Görünümü Sıfırla

### 📱 Responsive Tasarım
- Mobil cihazlarda uyumlu çalışma
- Farklı ekran boyutlarına adaptasyon
- Dokunmatik cihaz desteği

## Kurulum

1. **Dosya Yapısı**
   ```
   abko2606/
   ├── index_new.html
   ├── style_new.css
   ├── careerData.js
   ├── ogretmenVR.mp4  ← 360° VR video dosyası
   └── README_VR.md
   ```

2. **Gereksinimler**
   - Modern web tarayıcısı (Chrome, Firefox, Safari, Edge)
   - WebGL desteği
   - `ogretmenVR.mp4` dosyası proje klasöründe olmalı

3. **Çalıştırma**
   - `index_new.html` dosyasını web tarayıcısında açın
   - "Meslekleri İncele" bölümüne gidin
   - "Öğretmen" mesleğini seçin
   - "VR Simülasyonunu Başlat" butonuna tıklayın

## Teknik Detaylar

### Kullanılan Kütüphaneler
- **Three.js**: 3D grafik ve VR rendering
- **OrbitControls**: Kamera kontrolü
- **Bootstrap**: UI bileşenleri
- **Font Awesome**: İkonlar

### Video Formatı
- **Format**: MP4
- **Çözünürlük**: 360° (equirectangular)
- **Codec**: H.264
- **Önerilen**: 4K (3840x1920) veya 2K (1920x960)

### Performans Optimizasyonları
- Video texture caching
- Responsive canvas sizing
- Memory cleanup on page change
- Error handling ve fallback

## Kullanım

### Öğretmen Mesleği VR Deneyimi
1. Ana sayfada "Meslekleri İncele" seçeneğini seçin
2. "Öğretmen" mesleğini bulun
3. "VR Simülasyonunu Başlat" butonuna tıklayın
4. 360° VR video player açılacak
5. Fare ile etrafı keşfedin ve öğretmenlik mesleğini deneyimleyin

### Kontroller
- **Oynat/Duraklat**: Video oynatmayı kontrol eder
- **Tam Ekran**: Tam ekran moduna geçer
- **Görünümü Sıfırla**: Kamerayı başlangıç pozisyonuna döndürür

## Sorun Giderme

### Video Yüklenmiyor
- `ogretmenVR.mp4` dosyasının proje klasöründe olduğundan emin olun
- Dosya adının doğru yazıldığını kontrol edin
- Tarayıcı konsolunda hata mesajlarını kontrol edin

### Three.js Hatası
- Modern bir web tarayıcısı kullandığınızdan emin olun
- WebGL desteğini kontrol edin
- Sayfayı yenileyin

### Performans Sorunları
- Video dosyasının boyutunu küçültün
- Daha düşük çözünürlüklü video kullanın
- Tarayıcıyı güncelleyin

## Gelecek Geliştirmeler

- [ ] Diğer meslekler için VR video desteği
- [ ] VR gözlük uyumluluğu
- [ ] Ses kontrolü
- [ ] Video kalitesi ayarları
- [ ] Otomatik oynatma seçenekleri

## Lisans

Bu proje eğitim amaçlı geliştirilmiştir.

## İletişim

Sorularınız için proje sahibi ile iletişime geçebilirsiniz. 