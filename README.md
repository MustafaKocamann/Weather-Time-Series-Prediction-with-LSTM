# 🌦️ Zaman Serisi Tahmini: Jena Climate Dataset ile LSTM Uygulaması
📌 Proje Hakkında

Bu proje, Jena Climate veri seti kullanılarak zaman serisi tahmini yapmayı amaçlamaktadır.
Derin öğrenme tabanlı LSTM (Long Short-Term Memory) modeli ile sıcaklık tahmini gerçekleştirilmiştir.

## Proje Kapsamı

* Veri ön işleme

* Keşifsel Veri Analizi (EDA)

* Windowing (sliding window) yaklaşımı

* LSTM tabanlı model geliştirme

* Model optimizasyonu ve performans değerlendirmesi

## 📊 Veri Seti Hikayesi

Jena Climate veri seti, 1 Ocak 2009 – 31 Aralık 2016 tarihleri arasında, her 10 dakikada bir ölçülen iklim verilerini içermektedir.

## Özellikler

* Date Time → Ölçüm tarihi ve saati

* p (mbar) → Atmosfer basıncı

* T (°C) → Hava sıcaklığı

* Tpot (K) → Potansiyel sıcaklık

* Tdew (°C) → Çiy noktası sıcaklığı

* rh (%) → Bağıl nem

* VPmax (mbar) → Maksimum buhar basıncı

* VPact (mbar) → Gerçek buhar basıncı

* VPdef (mbar) → Buhar basıncı açığı

* sh (g/kg) → Özgül nem

* H2OC (mmol/mol) → Su buharı yoğunluğu

* rho (g/m³) → Hava yoğunluğu

* wv (m/s) → Ortalama rüzgar hızı

* max. wv (m/s) → Maksimum rüzgar hızı

* wd (°) → Rüzgar yönü

## 🛠️ Kullanılan Teknolojiler

* Python 3.9+

* TensorFlow / Keras – LSTM modeli

* NumPy & Pandas – Veri işleme

* Matplotlib & Seaborn – Görselleştirme

* scikit-learn – Ölçekleme ve metrikler

## 📐 Model Yaklaşımı

* Veri Hazırlığı → Zaman serisi formatına dönüştürme, windowing tekniği (5 adımlık pencere)

* LSTM Modeli → Çok katmanlı LSTM yapısı + Dropout katmanları

* Hiperparametre Ayarlamaları → Batch size, learning rate, optimizer (Adam)

* Callback’ler → EarlyStopping, ModelCheckpoint, ReduceLROnPlateau

* Değerlendirme → Eğitim, doğrulama ve test setleri üzerinde performans ölçümleri
