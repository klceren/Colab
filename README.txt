# ✈️ Uydu Görüntülerinden Otomatik Uçak Tespiti

Bu proje, uydu görüntülerini analiz ederek içerisinde uçak olup olmadığını tespit eden bir makine öğrenmesi modelidir. Proje kapsamında verinin ham halinden işlenmiş haline, görselleştirilmesinden model eğitimine kadar uçtan uca bir veri bilimi süreci yürütülmüştür.

## 🚀 Proje Özeti
- **Problem Türü:** İkili Sınıflandırma (Binary Classification)
- **Veri Seti:** Kaggle - PlanesNet (32,000 adet 20x20 RGB görüntü)
- **Teknoloji Yığını:** Python, Google Colab, NumPy, Matplotlib, Seaborn, Scikit-learn

## 🛠️ Yapılan İşlemler

### 1. Veri Hazırlama ve Reshape
Ham veriler 1200 piksellik düz listeler halindeydi. Bilgisayarlı görü (computer vision) prensiplerine uygun olarak veriler **20x20x3 (RGB)** formatına dönüştürüldü. Bu sayede her görüntü gerçek renkli bir resim yapısına kavuşturuldu.

### 2. Keşifsel Veri Analizi (EDA)
- **Eksik Değer Kontrolü:** Veri setinde `NaN` (boş) değer olup olmadığı kontrol edilerek veri bütünlüğü doğrulandı.
- **Sınıf Dağılımı:** Veri setindeki "Uçak Var" ve "Uçak Yok" sınıflarının dağılımı Seaborn kütüphanesi ile görselleştirildi.
- **Örnek Görselleştirme:** Rastgele seçilen veriler, etiketleriyle birlikte (Uçak/Değil) ekrana bastırılarak doğrulama yapıldı.

### 3. Model Eğitimi
Veri seti %80 eğitim ve %20 test olarak ikiye ayrıldı. **Lojistik Regresyon** algoritması kullanılarak model eğitildi ve test verisi üzerinde yüksek doğruluk oranı elde edildi.

## 📊 Sonuçlar
Model, uydu görüntülerindeki piksellerin renk yoğunluklarını ve yapılarını analiz ederek uçakları yüksek bir başarı oranıyla tespit edebilmektedir.

---
**Hazırlayan:** [Adın Soyadın]  
**Ders:** Yapay Zeka / Veri Bilimi Giriş  
**Üniversite:** İnönü Üniversitesi