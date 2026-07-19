# Softito Python & Yapay Zekâ Portföyü

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![Status](https://img.shields.io/badge/status-geliştiriliyor-F59E0B)
![License](https://img.shields.io/badge/license-MIT-green)

Softito Yapay Zekâ Yazılımcılığı eğitimi boyunca işlenen konuları, birbirinden farklı veri setleri ve gerçek iş problemleri üzerinde uygulayan çalıştırılabilir proje koleksiyonudur.

Bu repo [mucahitesaday/softito_python_ai](https://github.com/mucahitesaday/softito_python_ai) yapısını referans alır; kodlar, veri setleri, problem senaryoları ve açıklamalar özgündür.

## İçerik

| No | Bölüm | Proje | Veri seti |
|---:|---|---|---|
| 01 | Python Temelleri | Öğrenci başarı analizi | Students Performance (Kaggle) |
| 02 | İleri Python | Sipariş yönetim sistemi | Brazilian E-Commerce (Kaggle) |
| 03 | EDA | Otel rezervasyon analizi | Hotel Booking Demand (Kaggle) |
| 04 | Linear Regression | Ev fiyat tahmini | California Housing |
| 05 | Logistic Regression | Müşteri kaybı tahmini | Telco Customer Churn (Kaggle) |
| 06 | Klasik ML | Kalp hastalığı model karşılaştırması | Heart Disease (Kaggle) |
| 07 | Denetimsiz Öğrenme | AVM müşteri segmentasyonu | Mall Customers (Kaggle) |
| 08 | Anomali Tespiti | Kredi kartı dolandırıcılığı | Credit Card Fraud (Kaggle) |
| 09 | Model İzleme | Tahmin dağılımı ve drift kontrolü | Weather AUS (Kaggle) |
| 10 | Deep Learning | Moda ürünü sınıflandırma | Fashion-MNIST |
| 11 | Computer Vision | Trafik levhası tanıma | GTSRB |
| 12 | NLP | Haber kategorisi tahmini | AG News |
| 13 | LLM & RAG | Türkçe doküman arama | Özgün bilgi tabanı |
| 14 | MLOps & Docker | Uçtan uca tahmin servisi | Telco Churn |
| 15 | Big Data | Spark ile uçuş gecikme analizi | Flight Delay (Kaggle) |

## Repo yapısı

```text
sotfttio-python/
├── 01_Python_Temelleri/
├── 02_Ileri_Python/
├── 03_EDA/
├── 04_Linear_Regression/
├── 05_Logistic_Regression/
├── 06_Klasik_ML/
├── 07_Denetimsiz_Ogrenme/
├── 08_Anomali_Tespiti/
├── 09_Model_Izleme/
├── 10_Deep_Learning/
├── 11_Computer_Vision/
├── 12_NLP/
├── 13_LLM_RAG/
├── 14_MLOps_Docker/
├── 15_Big_Data/
├── datasets.yaml
├── requirements.txt
└── README.md
```

Her bölümde açıklamalı Python kodu bulunur. Kodlar mümkün olduğunda küçük bir yerleşik/örnek veriyle doğrudan çalışır; büyük Kaggle verileri için `datasets.yaml` içindeki kaynak kullanılır.

## Kurulum

```bash
git clone https://github.com/burcuduzen/sotfttio-python.git
cd sotfttio-python
python -m venv .venv
source .venv/bin/activate       # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Kaggle verilerini indirmek için:

```bash
pip install kagglehub
python download_datasets.py --list
python download_datasets.py telco_churn
```

## Çalıştırma örnekleri

```bash
python 03_EDA/hotel_booking_eda.py
python 04_Linear_Regression/california_housing.py
python 06_Klasik_ML/model_comparison.py
python 07_Denetimsiz_Ogrenme/customer_segmentation.py
python 12_NLP/news_classification.py
```

## Proje standardı

- Veri doğrulama ve eksik değer kontrolü
- Tekrarlanabilir sonuç için sabit `random_state`
- Train/test ayrımı ve veri sızıntısına karşı `Pipeline`
- Accuracy yanında F1, ROC-AUC, MAE/RMSE gibi probleme uygun metrikler
- Grafik ve model çıktılarının `outputs/` altında saklanması
- Türkçe açıklamalar ve sade fonksiyon yapısı

## Hazırlayan

**Burcu Düzen**  
Bilgisayar Mühendisliği — Yapay Zekâ ve Veri Bilimi
