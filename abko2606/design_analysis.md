# Gelecek Rotası - Yeni Tasarım Analizi ve Tasarım Dili

## 1. Genel Bakış

Sağlanan görseller, mevcut ABKÖ Meslek Keşif Platformu için modern, dinamik ve kullanıcı dostu bir arayüz önermektedir. Tasarım, özellikle genç kullanıcılara hitap eden canlı renkler, akıcı geçişler ve ilgi çekici görsel öğelerle zenginleştirilmiştir. Platformun ana amacı olan meslek keşfi ve VR simülasyonları, görsel olarak vurgulanmıştır.

## 2. Renk Paleti

Tasarım, derin mor ve canlı sarı/turuncu tonlarının hakim olduğu bir renk paleti kullanmaktadır. Bu kontrast, önemli öğeleri vurgulamak ve görsel hiyerarşi oluşturmak için etkilidir.

- **Ana Arka Plan**: Koyu mordan (muhtemelen #4B0082 veya benzeri) daha açık mor/pembe tonlarına doğru degrade geçişler. Bu, derinlik ve modern bir his katmaktadır.
- **Vurgu Renkleri**: Canlı sarı (#FFD700 veya benzeri) ve turuncu tonları (#FFA500 veya benzeri). Bu renkler, butonlar, başlıklar ve önemli metinler için kullanılarak dikkat çekicilik sağlamaktadır.
- **Metin Renkleri**: Açık renkli arka planlarda koyu metinler, koyu renkli arka planlarda açık renkli metinler (beyaz veya açık gri) kullanılmıştır. Başlıklar genellikle vurgu rengi olan sarı tonlarındadır.

## 3. Tipografi

Görsellerde kullanılan fontlar, modern ve okunaklı bir yapıya sahiptir. Başlıklar genellikle kalın ve büyük puntolarla, gövde metinleri ise daha ince ve standart boyutlarda kullanılmıştır. Bu, bilginin kolayca taranmasını ve okunmasını sağlar.

- **Başlıklar**: Kalın, sans-serif bir font (örneğin, Montserrat, Poppins veya benzeri). Büyük harf kullanımı yaygındır.
- **Gövde Metni**: Daha hafif, okunaklı bir sans-serif font (örneğin, Open Sans, Lato veya benzeri).

## 4. Düzen ve Yerleşim (Layout)

Tasarım, geniş ekranlarda merkezi yerleşimi ve mobil cihazlarda duyarlı (responsive) bir yapıyı hedeflemektedir. İçerik, kullanıcıyı yönlendirecek şekilde düzenlenmiştir.

- **Navigasyon Çubuğu**: Üst kısımda, sol tarafta logo ve sağ tarafta ana sayfa, hakkında gibi menü öğeleri bulunmaktadır. Sağ üst köşede ek ikonlar (muhtemelen ayarlar veya dil seçimi için) yer almaktadır.
- **Ana Sayfa**: Büyük, dikkat çekici bir başlık, altında kısa bir açıklama ve ana eylem butonu (örn. "Hadi Başlayalım!"). Sağ tarafta meslek keşfi temasını yansıtan illüstrasyonlar (VR gözlüklü çocuklar, gezegenler vb.) bulunmaktadır.
- **Eylem Seçim Sayfası ("Ne Yapmak İstersin?")**: Ortada iki büyük buton (örn. "Meslek Testini Başlat", "Meslekleri İncele"). Butonların yanında ilgili ikonlar (pano, VR gözlük) yer almaktadır.
- **Test Sayfaları**: Başlık ("Test Sayfaları") ve muhtemelen test sorularının yer alacağı alan. Görselde detaylı test arayüzü görünmemektedir, ancak genel tasarım diline uygun olacaktır.
- **Sonuç Sayfası**: Büyük bir başlık ("Test Sonuçlarına Göre Sana Uygun Meslekler"), altında muhtemelen meslek kartlarının veya özetlerin yer alacağı alan. "Bu meslekleri VR ile keşfet" gibi bir ana eylem butonu bulunmaktadır.
- **VR Simülasyon Sayfaları**: Mesleğe özel başlık (örn. "Doktorluk Mesleği Simülasyonu"), altında meslek tanımı ve bir video oynatıcı placeholder'ı. Alt kısımda "Ana Sayfaya Dön" ve "Diğer Meslekleri Gör" butonları yer almaktadır.
- **Hakkında Sayfası**: Sol tarafta başlık ve metin, sağ tarafta tematik bir illüstrasyon (VR gözlük). Metin, platformun amacını ve işleyişini açıklamaktadır.

## 5. UI Elemanları

- **Butonlar**: Büyük, yuvarlak köşeli, vurgu renklerinde (sarı/turuncu) ve belirgin gölge efektlerine sahip. Hover durumlarında renk değişimi veya hafif büyüme animasyonları beklenir.
- **İkonlar**: Font Awesome veya benzeri bir ikon kütüphanesinden alınmış, tasarıma uygun, modern ve sade ikonlar.
- **Görsel Öğeler**: Arka planda dalgalı, soyut desenler (muhtemelen SVG veya CSS ile oluşturulmuş). Ana sayfada ve VR simülasyon sayfalarında mesleklere özel illüstrasyonlar bulunmaktadır.
- **Video Placeholder**: VR simülasyon sayfalarında ortada büyük bir oynat butonu olan video alanı.

## 6. Animasyonlar ve Geçişler

Tasarım, kullanıcı deneyimini zenginleştirmek için akıcı animasyonlar ve geçişler içermektedir. Özellikle sayfa geçişlerinde ve buton etkileşimlerinde yumuşak animasyonlar beklenir.

## 7. Erişilebilirlik

Renk kontrastları ve font boyutları, WCAG standartlarına uygun olacak şekilde ayarlanmalıdır. Odak yönetimi ve klavye navigasyonu da göz önünde bulundurulmalıdır.

## 8. Teknik Uygulama Notları

- **HTML Yapısı**: Her sayfa için ayrı `section` veya `div` elementleri kullanılacak ve JavaScript ile sayfa geçişleri yönetilecektir (SPA yaklaşımı).
- **CSS**: Degrade arka planlar, gölge efektleri ve buton stilleri için modern CSS özellikleri kullanılacaktır. Animasyonlar için `transition` ve `animation` özellikleri kullanılacaktır.
- **JavaScript**: Sayfa geçişleri, test mantığı, sonuç hesaplama ve VR simülasyon modal/sayfa yönetimi için kullanılacaktır. Mevcut ABKÖ mantığı bu yeni arayüze entegre edilecektir.
- **Görsel Varlıklar**: Sağlanan görsellerdeki illüstrasyonlar (VR gözlüklü çocuklar, meslek ortamları vb.) kullanılacaktır. Eğer doğrudan kullanılamazsa, benzer tarzda placeholder görseller oluşturulabilir.

Bu analiz, yeni tasarımın temel öğelerini ve uygulanması gereken anahtar noktaları özetlemektedir. Sonraki aşamalarda bu tasarım dilini HTML, CSS ve JavaScript koduna dönüştürmeye başlanacaktır.

