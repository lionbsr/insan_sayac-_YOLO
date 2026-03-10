# YOLO ile Webcam İnsan Sayacı

Bu proje, YOLO nesne tespit modeli kullanılarak geliştirilmiş basit bir insan sayacı uygulamasıdır. Sistem, bilgisayarın webcam kamerasını kullanarak görüntüdeki insanları gerçek zamanlı olarak tespit eder ve toplam insan sayısını ekranda gösterir.

## Kullanılan Teknolojiler

- Python
- OpenCV
- YOLO (Ultralytics)
- NumPy

## Çalışma Mantığı

Program webcam üzerinden canlı görüntü alır. Her görüntü karesi YOLO modeli ile analiz edilir. Model tarafından tespit edilen nesneler arasından sadece **person (insan)** sınıfı seçilir. Tespit edilen insanlar sayılır ve toplam kişi sayısı ekranda gösterilir.

## Kurulum

Gerekli kütüphaneleri yüklemek için:

```bash
pip install opencv-python ultralytics numpy
python insan_sayaci.py
insan_sayaci/
├── insan_sayaci.py
├── README.md
