# Gözetimli ve Gözetimsiz Öğrenme ile Spam Sınıflandırma

Bu proje, **gözetimli öğrenme** algoritmaları (Lojistik Regresyon, Karar Ağaçları) ve **gözetimsiz öğrenme** algoritmaları (k-Means, Mini Batch k-Means) kullanarak e-posta spam tespiti üzerine odaklanmaktadır.

## Proje Genel Bakış
Bu projede, e-posta mesajlarını spam(1) veya ham(0) olarak sınıflandırmak için farklı makine öğrenimi tekniklerini inceliyoruz. Gözetimli modeller ve gözetimsiz kümeleme algoritmalarını kullanarak etkinliklerini karşılaştırıyoruz.

## Kullanılan Algoritmalar:
- **Gözetimli Öğrenme**:
  - Lojistik Regresyon
  - Karar Ağaçları
- **Gözetimsiz Öğrenme**:
  - k-Means
  - Mini Batch k-Means

## Veri Seti
Bu projede kullanılan veri seti, spam veya ham olarak sınıflandırılmış e-posta mesajlarını içermektedir. Metin özellikleri ön işlemden geçirilmiş ve TF-IDF vektörizasyonu ile sayısal forma dönüştürülmüştür.

## Sonuçlar:
- **Lojistik Regresyon Doğruluğu**: %98.27
- **Karar Ağaçları Doğruluğu**: %95.88
- **k-Means Doğruluğu**: %54.28
- **Mini Batch k-Means Doğruluğu**: %55.78

## Kaggle'da Nasıl Çalıştırılır:
1. [Kaggle](https://www.kaggle.com/) sitesine gidin.
2. Kaggle'da "Notebooks" bölümünde yeni bir notebook oluşturun.
3. Bu depodan `spam-detection-with-supervised-and-unsupervised.ipynb` notebook dosyasını Kaggle notebook'unuza yükleyin.
4. Her hücreyi adım adım çalıştırarak sınıflandırma modellerini çalıştırın.

## Sonuç:
Bu veri setimiz için en uygunu doğruluk oranlarını göz önüne aldığımızda Gözetimli Öğrenme algoritması olan Lojistik Regresyon olduğu görülmüştür.
