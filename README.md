# 📊 Telco Müşteri Kaybı Tahmini

Müşteri kaybını (churn) önceden tahmin eden, makine öğrenmesi tabanlı sınıflandırma projesi. Telco müşteri verisi üzerinde **Random Forest** ve **Logistic Regression** modelleri karşılaştırılmakta; riskli müşteri segmenti tespit edilerek aksiyon önerileri sunulmaktadır.

## 🎯 Problem Tanımı

Yeni bir müşteri kazanmak, mevcut müşteriyi elde tutmaktan **5-7 kat daha pahalıdır**. Bu proje şu soruya yanıt arar:

> *"Hangi müşteriler yakın vadede bizi terk edecek ve onları elde tutmak için ne yapabiliriz?"*

# 🚀 Projenin Öne Çıkan Özellikleri
🔍 Kapsamlı keşifsel veri analizi (EDA) <br>
🧹 Veri ön işleme ve özellik mühendisliği <br>
⚖️ SMOTE ile sınıf dengesizliğinin giderilmesi <br>
🌲 Random Forest ile tahmine dayalı modelleme <br>
📈 ROC-AUC, Precision, Recall ve F1-Score ile performans değerlendirmesi <br>
🎯 En riskli müşterilerin belirlenmesi <br>
💼 İş kararlarına dönüştürülebilir stratejik içgörüler <br>
# 📌 Proje Amacı
Telekom sektöründe müşteri kaybı, şirketlerin gelirini doğrudan etkileyen en önemli sorunlardan biridir. Yeni müşteri kazanmanın maliyeti, mevcut müşteriyi elde tutmaktan çok daha yüksektir. <br>
### Bu proje ile amaçlanan: <br>
-Müşteri kaybı riskini önceden tahmin etmek. <br>
-Riskli müşterileri erken tespit etmek. <br>
-Kişiselleştirilmiş kampanyalar geliştirmek. <br>
-Müşteri sadakatini artırmak. <br>
-Gelir kaybını azaltmaktır. <br>
# 🗂️ Veri Seti <br>
Kullanılan veri seti, telekom müşterilerine ait demografik bilgiler, abonelik detayları, hizmet kullanımı ve müşteri kaybı durumunu içermektedir.<br>
Temel değişkenler:<br>
- Müşteri süresi (tenure)<br>
- Aylık ödeme (MonthlyCharges)<br>
- Toplam ödeme (TotalCharges)<br>
- Sözleşme türü<br>
- İnternet hizmeti<br>
- Ek hizmetler<br>
- Ödeme yöntemi<br>
- Müşteri kaybı (Churn)<br>
# 🛠️ Kullanılan Teknolojiler<br>
- Python<br>
- Pandas<br>
- NumPy<br>
- Matplotlib<br>
- Seaborn<br>
- Scikit-learn<br>
- Imbalanced-learn (SMOTE)<br>
# 🤖 Modeller

## Logistic Regression (Baseline)
- Hızlı ve yorumlanabilir.
- StandardScaler ile normalleştirme uygulandı.
- Karşılaştırma referansı olarak kullanıldı.

## Random Forest (Ana Model)
- 300 karar ağacı, `max_depth=10`
- `class_weight='balanced'` ile dengesizlik yönetimi
- SMOTE ile desteklenen eğitim seti
### Avantajları:<br>
-Yüksek doğruluk sağlar.<br>
-Overfitting riskini azaltır.<br>
-Karmaşık ilişkileri öğrenebilir.<br>
-Özellik önem sıralaması sunar.<br>
-Kategorik ve sayısal verilerle iyi çalışır.<br>

## Dengesiz Veri Yönetimi — SMOTE
Azınlık sınıfı (~%27) yapay örneklerle dengelendi. SMOTE **yalnızca eğitim setine** uygulandı; test seti gerçek dağılımı korudu.

# ⚙️ Uygulanan Veri Bilimi Adımları<br>
## 1. Veri Ön İşleme<br>
-Eksik verilerin temizlenmesi<br>
-Veri tiplerinin dönüştürülmesi<br>
-Hedef değişkenin sayısallaştırılması<br>
## 2. Özellik Mühendisliği<br>
-Ortalama aylık harcama<br>
-Uzun dönem müşteri göstergesi<br>
-Yüksek aylık ödeme göstergesi<br>
-Hizmet yılı başına ödeme oranı<br>
## 3. Sınıf Dengesizliğinin Giderilmesi<br>
-SMOTE yöntemi kullanılarak churn eden müşteri sınıfı dengelenmiştir.<br>
## 4. Model Eğitimi<br>
-Eğitim/test veri ayrımı<br>
-Random Forest modelinin eğitilmesi<br>
-Logistic Regression modelinin eğitilmesi<br>
-Tahminleme<br>
-Verilerin ölçeklendirilmesi<br>
## 5. Model Değerlendirme<br>
-Confusion Matrix<br>
-ROC Curve<br>
-ROC-AUC Score<br>
-Classification Report<br>
-Precision-Recall Curve<br>
-Feature Importance Analizi<br>
# 📈 Değerlendirme Metrikleri<br>
🎯Precision: Pozitif tahminlerin doğruluk oranı<br>
🔍Recall: Gerçek churn müşterilerini yakalama oranı<br>
⚖️F1-Score: Precision ve Recall'un dengeli ortalaması<br>
📈ROC-AUC: Modelin ayırt etme başarısı<br>
📉Average Precision (AP): Dengesiz veri setlerinde model performansını daha doğru ölçer<br>
# 🎯 İş Değeri ve Stratejik Katkılar
### Bu proje sayesinde şirketler:
Churn riski yüksek müşterileri önceden belirleyebilir.<br>
Kişiye özel kampanyalar oluşturabilir.<br>
Müşteri kaybını azaltabilir.<br>
Pazarlama bütçesini daha verimli kullanabilir.<br>
Müşteri yaşam boyu değerini artırabilir.<br>
# 📌 Önerilen Aksiyonlar<br>
🎁 Riskli müşterilere özel teklifler sunulması<br>
📲 Aktif olmayan müşterilere yeniden etkileşim kampanyaları<br>
💎 Sadakat programlarının güçlendirilmesi<br>
☎️ Yüksek değerli müşterilere birebir iletişim sağlanması<br>
📊 Risk skoru tabanlı müşteri segmentasyonu yapılması<br>
# 📊 Beklenen Sonuçlar<br>
📉 Müşteri kaybında azalma<br>
📈 Gelir artışı<br>
😊 Daha yüksek müşteri memnuniyeti<br>
🤝 Güçlü müşteri bağlılığı<br>
🎯 Daha verimli pazarlama stratejileri<br>
🧠 Veri odaklı karar alma kültürünün güçlenmesi<br>
