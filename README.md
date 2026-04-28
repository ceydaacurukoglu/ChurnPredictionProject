📊 Telco Müşteri Kaybı Tahmini

Telekomünikasyon sektöründe müşteri kaybını (churn) tahmin etmek için geliştirilmiş kapsamlı bir makine öğrenmesi projesidir. Bu proje, hizmeti bırakma riski taşıyan müşterileri belirlemeye ve proaktif müşteri tutundurma stratejileri geliştirmeye yardımcı olur.

🚀 Projenin Öne Çıkan Özellikleri
🔍 Kapsamlı keşifsel veri analizi (EDA)
🧹 Veri ön işleme ve özellik mühendisliği
⚖️ SMOTE ile sınıf dengesizliğinin giderilmesi
🌲 Random Forest ile tahmine dayalı modelleme
📈 ROC-AUC, Precision, Recall ve F1-Score ile performans değerlendirmesi
🎯 En riskli müşterilerin belirlenmesi
💼 İş kararlarına dönüştürülebilir stratejik içgörüler
📌 Proje Amacı

Telekom sektöründe müşteri kaybı, şirketlerin gelirini doğrudan etkileyen en önemli sorunlardan biridir. Yeni müşteri kazanmanın maliyeti, mevcut müşteriyi elde tutmaktan çok daha yüksektir.

Bu proje ile amaçlanan:

Müşteri kaybı riskini önceden tahmin etmek
Riskli müşterileri erken tespit etmek
Kişiselleştirilmiş kampanyalar geliştirmek
Müşteri sadakatini artırmak
Gelir kaybını azaltmaktır
🗂️ Veri Seti

Kullanılan veri seti, telekom müşterilerine ait demografik bilgiler, abonelik detayları, hizmet kullanımı ve müşteri kaybı durumunu içermektedir.

Temel değişkenler:

Müşteri süresi (tenure)
Aylık ödeme (MonthlyCharges)
Toplam ödeme (TotalCharges)
Sözleşme türü
İnternet hizmeti
Ek hizmetler
Ödeme yöntemi
Müşteri kaybı (Churn)
🛠️ Kullanılan Teknolojiler
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Imbalanced-learn (SMOTE)
🤖 Kullanılan Makine Öğrenmesi Modeli
Random Forest Classifier

Random Forest, birden fazla karar ağacının birleşiminden oluşan güçlü bir topluluk öğrenme algoritmasıdır.

Avantajları:

Yüksek doğruluk sağlar
Overfitting riskini azaltır
Karmaşık ilişkileri öğrenebilir
Özellik önem sıralaması sunar
Kategorik ve sayısal verilerle iyi çalışır
⚙️ Uygulanan Veri Bilimi Adımları
1. Veri Ön İşleme
Eksik verilerin temizlenmesi
Veri tiplerinin dönüştürülmesi
Hedef değişkenin sayısallaştırılması
2. Özellik Mühendisliği
Ortalama aylık harcama
Uzun dönem müşteri göstergesi
Yüksek aylık ödeme göstergesi
Hizmet yılı başına ödeme oranı
3. Sınıf Dengesizliğinin Giderilmesi
SMOTE ile azınlık sınıfının dengelenmesi
4. Model Eğitimi
Eğitim/test veri ayrımı
Random Forest model kurulumu
Tahminleme
5. Model Değerlendirme
Confusion Matrix
ROC Curve
ROC-AUC Score
Classification Report
📈 Değerlendirme Metrikleri
Precision: Pozitif tahminlerin doğruluk oranı
Recall: Gerçek churn müşterilerini yakalama oranı
F1-Score: Precision ve Recall'un dengeli ortalaması
ROC-AUC: Modelin ayırt etme başarısı
🎯 İş Değeri ve Stratejik Katkılar

Bu proje sayesinde şirketler:

Churn riski yüksek müşterileri önceden belirleyebilir
Kişiye özel kampanyalar oluşturabilir
Müşteri kaybını azaltabilir
Pazarlama bütçesini daha verimli kullanabilir
Müşteri yaşam boyu değerini artırabilir
📌 Önerilen Aksiyonlar
🎁 Riskli müşterilere özel teklifler sunulması
📲 Aktif olmayan müşterilere yeniden etkileşim kampanyaları
💎 Sadakat programlarının güçlendirilmesi
☎️ Yüksek değerli müşterilere birebir iletişim sağlanması
📊 Risk skoru tabanlı müşteri segmentasyonu yapılması
📊 Beklenen Sonuçlar
Müşteri kaybında azalma
Gelir artışı
Daha yüksek müşteri memnuniyeti
Güçlü müşteri bağlılığı
Veri odaklı karar alma kültürü
