# neural_networks_midterm_assignment
Masters level Neural Networks midterm assignment using the Breast Cancer dataset

**Proje Başlığı: MLP Sınıflandırma ve SHAP ile Açıklanabilir Yapay Zeka (XAI) Analizi**
Bu proje, Üsküdar Üniversitesi Yapay Sinir Ağları dersi ara sınav ödevi kapsamında geliştirilmiş olup, bir scikit-learn veri seti (örneğin Breast Cancer Wisconsin veya Wine Classification) üzerinde Multilayer Perceptron (MLP) tabanlı bir sınıflandırma modeli kurmayı ve bu modelin karar mekanizmasını SHAP (SHapley Additive exPlanations) yöntemiyle analiz etmeyi amaçlamaktadır.

🎯 **Amaç ve Kapsam**

Veri Bilimi Süreci: Seçilen veri seti üzerinde eksik değer, aykırı değer analizi ve ölçeklendirme gibi kapsamlı veri ön işleme adımlarını uygulamak.


Model Geliştirme: Farklı mimarilere (Basit, Orta, Geniş, Derin, Düşük Öğrenme Oranlı) sahip 5 adet MLP sınıflandırıcı modeli oluşturmak.



Hiperparametre Optimizasyonu: Optuna kütüphanesi ile otomatik hiperparametre optimizasyonu yaparak en iyi modeli bulmak.




Performans Değerlendirmesi: Tüm modelleri Accuracy, Precision, Recall, F1-Score ve ROC-AUC gibi metriklerle Validation ve Test setleri üzerinde değerlendirmek.



Açıklanabilir Yapay Zeka (XAI): Hem manüel hem de Optuna ile bulunan en iyi modellerin kararlarını SHAP analizi ile yorumlamak.

🛠️ **Kullanılan Teknolojiler**
Programlama Dili: Python

**Kütüphaneler:**

Veri Manipülasyonu: pandas, numpy

Makine Öğrenimi: scikit-learn (özellikle MLPClassifier)

Hiperparametre Optimizasyonu: Optuna

XAI (Açıklanabilirlik): SHAP

Veri Görselleştirme: matplotlib, seaborn

📝 **Uygulanan Adımlar ve Ana Sonuçlar**
Proje adımları, ödev yönergesine tam uygun olarak tamamlanmıştır.

1. **Veri Hazırlama ve EDA (Keşifsel Veri Analizi)**

Veri Seti: Seçilen veri seti: [Veri Seti Adını Buraya Ekleyin, örn: Breast Cancer Wisconsin].


Ön İşleme: Eksik değerler [uygulanan yöntem, örn: ortalama ile] doldurulmuş, aykırı değerler [uygulanan yöntem, örn: Z-Score] ile incelenmiştir.



Ölçeklendirme: Özellikler, StandardScaler kullanılarak ölçeklendirilmiştir.


Veri Bölünmesi: Veri seti %70 Eğitim, %10 Validasyon ve %20 Test olarak ayrılmıştır.

2. **MLP Modelleri ve Karşılaştırma**
5 farklı MLP mimarisi (Basit, Orta, Geniş, Derin, Düşük Öğrenme Oranlı) kurulmuş ve Validasyon seti üzerinde performansları karşılaştırılmıştır.



En İyi Manüel Model: Model [Model Numarası] ([Model Adı, örn: Derin]) validasyon setinde en yüksek [Metrik, örn: F1-Score] değerine ulaşmıştır.

Validation Karşılaştırma Tablosu, [Dosya/Görsel Adı] içinde mevcuttur.

3. **Optuna ile Hiperparametre Optimizasyonu**
150 deneme ile Optuna kullanılarak gizli katman boyutları, aktivasyon fonksiyonu, öğrenme oranı, regülarizasyon (alpha) ve çözücü (solver) parametreleri optimize edilmiştir.



Optuna En İyi Model Parametreleri:

hidden_layer_sizes: (X, Y)

learning_rate_init: Z

activation: [relu/tanh]

... (Diğer önemli parametreleri ekleyin)

4. **En İyi Modelin Test Performansı**
Validasyon sonuçlarına göre seçilen veya Optuna ile bulunan en iyi model, Test seti üzerinde değerlendirilmiştir.


Test Metrikleri:

Accuracy: [Değer]%

F1-Score: [Değer]

ROC-AUC: [Değer]


Görsel Çıktılar: Confusion Matrix ve ROC Eğrisi çizilmiştir.


5. **XAI – SHAP Açıklanabilirlik Analizi**
En iyi modeller için SHAP analizleri yapılarak özelliklerin kararlara katkısı belirlenmiştir.



Baskın Özellikler (SHAP): Analizlere göre en baskın 3 özellik: [Özellik 1], [Özellik 2] ve [Özellik 3] olarak belirlenmiştir.

**Görsel Çıktılar:**

summary_plot (Genel Etki)

bar_plot (Özellik Önem Sıralaması)

force_plot (Tekil Örnek Açıklaması)

decision_plot (Karar Yolu Katkısı)
