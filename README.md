# AIC 502 - Makine Öğrenmesi Ara Sınav Ödevi

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ypMl6oh6TMENteG8vZt9MNxCbBEwiu3W?usp=sharing)

## 📋 Proje Hakkında

Bu proje, Topkapı Üniversitesi Yapay Zeka Yüksek Lisans programı kapsamında hazırlanan Makine Öğrenmesi ara sınav ödevidir. Projede scikit-learn Wine veri seti üzerinde klasik makine öğrenmesi algoritmaları kullanılarak sınıflandırma modelleri kurulmuş, PCA ve LDA ile boyut indirgeme yapılmış ve SHAP ile açıklanabilir yapay zeka (XAI) analizi gerçekleştirilmiştir. 

**Öğrenci:** Vedat Sinan Ural  
**Öğrenci No:** 25221001010  
**Program:** Yapay Zeka Y.L. (Tezli)

## 📊 Veri Seti

- **Veri Seti:** Wine Classification (scikit-learn)
- **Örnek Sayısı:** 178
- **Özellik Sayısı:** 13
- **Sınıf Sayısı:** 3

## 🔬 Uygulanan Yöntemler

### Veri Ön İşleme
- Eksik değer analizi
- Aykırı değer tespiti (IQR ve Z-score)
- Veri ölçeklendirme (StandardScaler)

### Boyut İndirgeme
- **PCA** (Principal Component Analysis)
- **LDA** (Linear Discriminant Analysis)

### Makine Öğrenmesi Modelleri
Her üç veri temsili (Ham, PCA, LDA) için aşağıdaki modeller eğitilmiştir:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. XGBoost Classifier
5. Naive Bayes (GaussianNB)

**Toplam:** 15 model

### Değerlendirme Metrikleri
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

### XAI - Açıklanabilir Yapay Zeka
- SHAP (SHapley Additive exPlanations) analizi
- Özellik önemi görselleştirmeleri
- PCA vs LDA SHAP karşılaştırması

## 🏆 Sonuçlar

En iyi performans gösteren modeller (%100 accuracy):
- LR_Raw (Logistic Regression - Ham Veri)
- LR_LDA
- DT_LDA
- RF_LDA
- XGB_PCA
- NB_LDA

**Seçilen En İyi Model:** LR_Raw (Logistic Regression - Ham Veri)

## 🚀 Çalıştırma

### Google Colab (Önerilen)
Yukarıdaki "Open in Colab" butonuna tıklayarak notebook'u doğrudan çalıştırabilirsiniz.

### Yerel Ortam
```bash
# Repository'yi klonlayın
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO

# Gereksinimleri yükleyin
pip install -r requirements.txt

# Jupyter Notebook'u başlatın
jupyter notebook ML_arasinav.ipynb
```

## 📦 Gereksinimler

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- shap
- scipy

## 📁 Dosya Yapısı

```
├── README.md
├── requirements.txt
└── ML_arasinav.ipynb
```

## 📝 Lisans

Bu proje eğitim amaçlı hazırlanmıştır.
