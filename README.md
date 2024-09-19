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

## Alternatif
Projeyi doğrudan Kaggle üzerinden çalıştırmak için şu linki kullanabilirsiniz: [spam-detection Kaggle Notebook](https://www.kaggle.com/code/kubilaiswf/spam-detection-with-supervised-and-unsupervised)

## Sonuç:
Bu veri setimiz için en uygunu doğruluk oranlarını göz önüne aldığımızda Gözetimli Öğrenme algoritması olan Lojistik Regresyon olduğu görülmüştür.

Bu nedenle, Lojistik Regresyon modelini optimize etmeye çalıştım. **GridSearchCV** kullanarak `C` ve `penalty` parametrelerini optimize ettim. Optimizasyon sonucunda, doğruluk oranı hafif bir şekilde %98.27'den **%98.53**'e yükseldi. Kesinlik (%98.42), duyarlılık (%98.21) ve F1 skoru (%98.31) da optimize edilerek modelin genel performansı iyileştirildi.

- **Doğruluk (Accuracy)**: %98.53
- **Kesinlik (Precision)**: %98.42
- **Duyarlılık (Recall)**: %98.21
- **F1 Skoru**: %98.31

Bu iyileştirme sonucunda, **Lojistik Regresyon** modelinin, e-posta spam sınıflandırmasında en etkili yöntem olduğu görülmüştür.
