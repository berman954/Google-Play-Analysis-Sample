
Google Play Store Uygulama Analizi: Veri Temizleme, Modelleme ve Popülerlik Tahmini📱📊


1. 📌 Veri Temizleme ve Ön İşleme (Data Preprocessing)
   ✅ Eksik veri doldurma (missing value imputation) işlemleri yapıldı. Özellikle **Rating** sütunundaki eksik değerler, veri setinin ortalama değeriyle dolduruldu.  
   ✅ Sayısal olmayan sütunlar sayısal verilere dönüştürüldü. **Reviews** ve **Installs** sütunlarındaki karakterler temizlendi ve sayısal formatta işlem yapabilmek için dönüştürüldü.  
   ✅ Popülerlik tahmini için **Popularity** değişkeni oluşturuldu ve 1 milyonun üzerinde indirilen uygulamalar popüler olarak işaretlendi.  
  
2. 📊 Keşifsel Veri Analizi (EDA) ve Görselleştirme
   ✅ **İnceleme Sayıları** ve **Uygulama Kategorileri** gibi temel değişkenler görselleştirildi.  
   ✅ Uygulamaların popülerliği ile ilişkili **Kategorik Değişkenlerin** analizi yapıldı ve her kategoriye ait uygulama sayıları görselleştirildi.  
   
3. ⚙️ Özellik Mühendisliği (Feature Engineering & Feature Selection)
   ✅ Veri setindeki özellikler, popülerlik tahminine yönelik olarak seçildi. **Reviews** ve **Installs** gibi bağımsız değişkenler kullanıldı.  
   
4. 🤖 Model Seçimi ve Eğitimi (Model Selection & Training)
   ✅ Lojistik Regresyon (Logistic Regression) modeli ile popülerlik tahmin edildi. Model, **Reviews** ve **Installs** gibi değişkenlerle eğitildi ve sonuçlar değerlendirildi.  
   ✅ Modelin bağımlı ve bağımsız değişkenler ile olan ilişkisi incelendi.  

5. 📉 Model Değerlendirme (Evaluation Metrics)
   ✅ **Confusion Matrix** kullanılarak modelin doğruluğu ve performansı ölçüldü.  
   ✅ **Accuracy** ve **Precision-Recall** analizleri yapıldı.  
   Eksik: ROC-AUC eğrisi ve SHAP analizi yapılmadı.

6. 🔬 Model Doğrulama (Cross-Validation & Generalization)
   ✅ Eğitim ve test verileri arasında **%70 - %30** ayrım yapılarak modelin doğruluğu test edildi.  
   ✅ Modelin genellenebilirliğini test etmek amacıyla eğitim seti üzerinde doğruluk oranları hesaplandı.

SONUÇ:
Veri Analizi: Welch t-testinden elde edilen sonuç, Reviews sayılarındaki farkın anlamlı olduğunu gösteriyor.

Modelleme: Lojistik regresyon modelinin başarılı bir uyum sağladığını ancak Reviews ve Installs değişkenlerinin modelde yer almadığını ve bu değişkenlerin birbirleriyle yüksek derecede ilişkili olabileceğini gösteriyor. Bu, modelin daha sağlam ve doğru sonuçlar verebilmesi için değişken seçimi veya multicollinearity kontrolü yapılması gerektiği düşünülebilir.
   
   
   ################################ENG##############


Google Play Store App Analysis: Data Cleaning, Modeling, and Popularity Prediction 📱📊



1. 📌 Data Cleaning and Preprocessing
   ✅ Missing value imputation was performed, particularly filling in missing values in the **Rating** column with the mean value of the dataset.  
   ✅ Non-numeric columns were converted to numeric. Special characters in the **Reviews** and **Installs** columns were cleaned and converted into numerical values for analysis.  
   ✅ A new **Popularity** variable was created, marking apps with over 1 million installs as popular.  
  
2. 📊 Exploratory Data Analysis (EDA) and Visualization
   ✅ **Review Counts** and **App Categories** were visualized to understand data distributions.  
   ✅ The distribution of apps across different categories was plotted, providing insights into the number of apps per category.  
   Missing: Boxplots, histograms, and feature importance analysis were not detailed.

3. ⚙️ Feature Engineering & Feature Selection
   ✅ Relevant features for popularity prediction were selected, including **Reviews** and **Installs** as key predictors.  
   Missing: New engineered features were not created.

4. 🤖 Model Selection and Training
   ✅ A **Logistic Regression** model was trained to predict app popularity, using features like **Reviews** and **Installs**.  
   ✅ The relationship between the dependent and independent variables was explored.

5. 📉 Model Evaluation
   ✅ Model performance was evaluated using a **Confusion Matrix**.  
   ✅ **Accuracy**, **Precision**, and **Recall** metrics were calculated to assess the model's performance.  
   Missing: ROC-AUC curve and SHAP analysis were not performed.

6. 🔬 Model Validation (Cross-Validation & Generalization)
   ✅ The dataset was split into **70% training** and **30% test** sets to evaluate the model's accuracy.  
   ✅ The model's generalization ability was tested, and accuracy was measured on the test set.
