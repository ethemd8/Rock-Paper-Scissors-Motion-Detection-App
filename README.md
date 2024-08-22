# **Taş Kağıt Makas Hareket Tespit Uygulaması**

Bu proje, bir kameradan alınan görüntüleri kullanarak taş, kağıt, makas oyununda yapılan el hareketlerini tespit eden bir uygulama sunar. Uygulama, YOLO modeli ile görüntüdeki el hareketlerini algılar ve gerçek zamanlı olarak sınıflandırır.

## **Özellikler**

- **Gerçek Zamanlı Hareket Tespiti**: Kamera görüntüsü üzerinden el hareketleri anında tespit edilir.
- **Sınıflandırma**: Algılanan el hareketleri taş, kağıt veya makas olarak sınıflandırılır.
- **FPS Takibi**: Gerçek zamanlı performans değerlendirmesi için FPS (Frame Per Second) görüntüleme.
- **Kullanıcı Etkileşimi**: Kısayol tuşları ile video oynatım kontrolü (`q` çıkış, `s` ileri sarma, `space` duraklatma).

## **Kurulum**

1. **Gerekli Kütüphaneleri Yükleyin**:
   ```bash
   pip install ultralytics opencv-python cvzone numpy
Proje Dosyalarını İndirin:

bash
Kodu kopyala
git clone https://github.com/kullaniciadi/tas-kagit-makas-detect.git
Model Ağırlıklarını Ekleyin: yoloWeight klasörüne best8N.pt dosyasını ekleyin.

Uygulamayı Çalıştırın:

bash
Kodu kopyala
python rps_detect.py
Kullanım
Kamera Seçimi: cap = cv2.VideoCapture(0) ile varsayılan web kameranızı kullanabilirsiniz.
Video Modu (Opsiyonel): cap = cv2.VideoCapture("../Videos/motorbikes.mp4") satırını açarak video dosyası üzerinden de test yapabilirsiniz.
Sonuçları Görüntüleme: Hareket tespitini ve sınıflandırmayı anlık olarak ekranınızda görebilirsiniz.
Ekran Görüntüleri

![image](https://github.com/user-attachments/assets/6658c5fb-2f2b-4567-861f-bb8ca0f5c4e4)

Tespit edilen el hareketi ve sınıflandırma sonucu.

Kullanılan Teknolojiler
[eğitim seti]([https://www.google.com](https://universe.roboflow.com/team-roboflow/rock-paper-scissors-detection/dataset/44))

YOLO Modeli: Hareket tespiti için.
OpenCV: Görüntü işleme ve video analizi.
cvzone: Tespit edilen objeleri görsel olarak işaretlemek için.
Gelecek Geliştirmeler
İyileştirilmiş Model: Daha yüksek doğruluk oranı için model optimizasyonu.
Yeni Hareketler: Farklı el hareketleri veya jestler için sınıflandırma desteği.
Mobil Entegrasyon: Uygulamanın mobil cihazlar için optimize edilmesi.
