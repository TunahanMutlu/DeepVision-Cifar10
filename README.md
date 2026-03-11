# Deep Vision - CIFAR-10 Image Classifier

## Proje Özeti
Bu depo, CIFAR-10 veri seti kullanılarak eğitilmiş bir Evrişimli Sinir Ağı (CNN) modelini içermektedir. Projenin temel amacı, TensorFlow ve Keras kütüphaneleri kullanılarak temel görüntü sınıflandırma mimarilerinin nasıl kurulduğunu uygulamalı olarak göstermektir. Geliştirilen bu model, otonom sistemlerdeki nesne tespiti ve görsel veri işleme görevleri için bir altyapı niteliği taşımaktadır.

## Kullanılan Teknolojiler
* Python
* TensorFlow / Keras
* Jupyter Notebook

## Model Mimarisi
Model, $32 \times 32$ piksel boyutlarındaki giriş görüntülerini işleyip 10 farklı sınıftan birine ayırmak üzere tasarlanmıştır. Mimari özetle şu katmanlardan oluşur:
* Özellik çıkarımı için ardışık `Conv2D` ve `MaxPooling2D` katmanları.
* Çok boyutlu veriyi tek boyutlu vektöre dönüştüren `Flatten` katmanı.
* Sınıflandırma işlemini gerçekleştiren `Dense` (Tam Bağlı) katmanlar (Çıkış katmanı 10 nörona sahiptir).

## Dosya Yapısı
* `DeepVision_Cifar10.ipynb`: Veri setinin yüklenmesi, CNN modelinin inşa edilmesi, eğitilmesi ve performansının test edilmesini içeren ana çalışma dosyasıdır.
