Rain in Australia Prediction | Team Shinning Stars

FET445 - Veri Madenciliği (İstanbul Topkapı Üniversitesi)  
2024-2025 Güz  
Avustralya Meteoroloji Verileri ile Yağmur Tahmini (Sınıflandırma)

Bu proje, Avustralya genelindeki birçok istasyondan alınan 10 yıllık günlük hava durumu gözlemlerini kullanarak, "Yarın yağmur yağacak mı?" sorusuna makine öğrenmesi yöntemleriyle cevap aramaktadır.

Veri setindeki sınıf dengesizliği (Imbalanced Data) ve mevsimsel etkiler göz önüne alınarak; Logistic Regression, Random Forest, Decision Tree ve XGBoost algoritmaları karşılaştırmalı olarak analiz edilmiştir.

Sınıflandırma: `RainTomorrow` değişkenini (Yes/No) tahmin etmek.
Başarı Kriteri: Dengesiz veri setinde sadece Doğruluk (Accuracy) değil, F1-Score ve ROC-AUC değerlerini maksimize etmek.
Veri Etiği: `RISK_MM` gibi veri sızıntısına (Data Leakage) yol açan öznitelikleri tespit edip temizlemek.

---

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
│   ├── TeamShinningStars_DataPreparation.ipynb # Ortak Veri Analizi ve Temizlik
│   ├── YUSUF_RIDVAN_CELIKBAS_22040101055_TeamShinningStars.ipynb  # Logistic Regression
│   ├── AYCA_SU_YILDIRIM_22040101049_TeamShinningStars.ipynb  # Random Forest
│   ├── MUHAMMED_EFE_KUCUKYETER_22040101042_TeamShinningStars.ipynb  # Decision Tree
│   └── EMRE_SOMER_CABAK_22040101027_TeamShinningStars.ipynb  # XGBoost vs Bagging
│
├── YUSUF_RIDVAN_CELIKBAS_22040101055_TeamShinningStars.pdf.  # Proje İlerleme Raporu (PDF)
└── README.md                           # Proje dokümantasyonu (Bu dosya)

---

Ekip Üyeleri ve Görev Dağılımı (Team Shinning Stars)

| Öğrenci No | Ad Soyad | Rol / Sorumlu Olduğu Model |
| :--- | :--- | :--- |
| **22040101055** | **Yusuf Rıdvan Çelikbaş** | Doğrusal Modeller (Logistic Regression) & Veri Ölçekleme |
| **22040101049** | **Ayça Su Yıldırım** | Topluluk Öğrenmesi (Random Forest) & EDA |
| **22040101042** | **Muhammed Efe Küçükyeter** | Karar Ağaçları (Decision Tree) & Özellik Mühendisliği |
| **22040101027** | **Emre Somer Çabak** | Gelişmiş Modeller (XGBoost & Bagging) & Karşılaştırma |
