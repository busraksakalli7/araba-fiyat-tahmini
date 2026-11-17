# Mercedes-Benz Fiyat Tahmin Modeli (Deep Learning)

Bu proje, TensorFlow ve Keras kütüphaneleri kullanılarak geliştirilmiş bir Yapay Sinir Ağı (ANN) regresyon modelidir. Mercedes ikinci el araç veri seti kullanılarak araç özelliklerine göre fiyat tahmini yapılması amaçlanmıştır.

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler
* Python
* TensorFlow / Keras
* Pandas & NumPy
* Scikit-Learn
* Matplotlib & Seaborn

## 📈 Proje Adımları
1. **Veri Ön İşleme ve Keşifsel Veri Analizi (EDA):** Eksik verilerin kontrolü, korelasyon matrisi incelemesi.
2. **Aykırı Değer (Outlier) Temizliği:** Fiyat dağılımını optimize etmek için en yüksek fiyatlı %1'lik dilimin çıkarılması.
3. **Ölçeklendirme (Scaling):** `MinMaxScaler` ile verilerin normalize edilmesi
4. **Model Mimarisi:** Katmanlı Yapay Sinir Ağı (Dense layers) kurulumu ve model eğitimi.
5. **Model Değerlendirme:** MSE ve RMSE metrikleri ile hata payının analiz edilmesi.

## 🚀 Modeli Çalıştırma
Kaydedilen modeli (`merc_model.keras`) yükleyerek yeni araç verileriyle tahmin yaptırabilirsiniz:
```python
from tensorflow.keras.models import load_model

model = load_model("merc_model.keras")
# tahmin = model.predict(yeni_veri)
