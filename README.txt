# 🌧️ Rain in Australia Prediction | Team Shinning Stars

**Ders:** FET445 - Veri Madenciliği (İstanbul Topkapı Üniversitesi)  
**Dönem:** 2024-2025 Güz  
**Proje Konusu:** Avustralya Meteoroloji Verileri ile Yağmur Tahmini (Sınıflandırma)

---

## 📌 Proje Hakkında
Bu proje, Avustralya genelindeki birçok istasyondan alınan 10 yıllık günlük hava durumu gözlemlerini kullanarak, **"Yarın yağmur yağacak mı?"** sorusuna makine öğrenmesi yöntemleriyle cevap aramaktadır.

Veri setindeki sınıf dengesizliği (Imbalanced Data) ve mevsimsel etkiler göz önüne alınarak; **Logistic Regression**, **Random Forest**, **Decision Tree** ve **XGBoost** algoritmaları karşılaştırmalı olarak analiz edilmiştir.

### 🎯 Hedefler
* **Sınıflandırma:** `RainTomorrow` değişkenini (Yes/No) tahmin etmek.
* **Başarı Kriteri:** Dengesiz veri setinde sadece Doğruluk (Accuracy) değil, **F1-Score** ve **ROC-AUC** değerlerini maksimize etmek.
* **Veri Etiği:** `RISK_MM` gibi veri sızıntısına (Data Leakage) yol açan öznitelikleri tespit edip temizlemek.

---

## 👥 Ekip Üyeleri ve Görev Dağılımı (Team Shinning Stars)

| Öğrenci No | Ad Soyad | Rol / Sorumlu Olduğu Model |
| :--- | :--- | :--- |
| **22040101055** | **Yusuf Rıdvan Çelikbaş** | Doğrusal Modeller (Logistic Regression) & Veri Ölçekleme |
| **22040101049** | **Ayça Su Yıldırım** | Topluluk Öğrenmesi (Random Forest) & EDA |
| **22040101042** | **Muhammed Efe Küçükyeter** | Karar Ağaçları (Decision Tree) & Özellik Mühendisliği |
| **22040101027** | **Emre Somer Çabak** | Gelişmiş Modeller (XGBoost & Bagging) & Karşılaştırma |

---

## 📂 Klasör Yapısı
Proje dosyalarımız aşağıdaki düzende organize edilmiştir:

```text
FET445_TeamShinningStars/
├── dataset/
│   ├── weatherAUS.csv             # Orijinal Kaggle veri seti
│   └── cleaned_weather_vize.csv   # Ön işleme yapılmış, temizlenmiş veri
│
├── images/                        # Rapor ve sunumda kullanılan grafikler
│   ├── grafik1_dagilim.png
│   ├── grafik2_heatmap.png
│   └── ...
│
├── notebooks/                     # Jupyter Notebook Kod Dosyaları
│   ├── 0_Master_EDA_and_Cleaning.ipynb               # Ortak Veri Analizi ve Temizlik
│   ├── FET445_22040101055_TeamShinningStars_1.ipynb  # Logistic Regression
│   ├── FET445_22040101049_TeamShinningStars_2.ipynb  # Random Forest
│   ├── FET445_22040101042_TeamShinningStars_3.ipynb  # Decision Tree
│   └── FET445_22040101027_TeamShinningStars_4.ipynb  # XGBoost vs Bagging
│
├── FET445_..._ProjectOutline.pdf.docx  # Proje İlerleme Raporu (Word/PDF)
├── .gitignore                          # Git tarafından izlenmeyecek dosyalar
└── README.md                           # Proje dokümantasyonu (Bu dosya)