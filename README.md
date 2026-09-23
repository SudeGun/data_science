# Data Science & Analytics Projects

Bu repo, **AIN 214: Data Science and Analytics** dersi kapsamında tamamladığım veri ön işleme, ilişkisel veri tabanı tasarımı (SQL), keşifçi veri analizi (EDA), makine öğrenmesi (Regresyon & Sınıflandırma) ve veri görselleştirme projelerini içermektedir.

---

## 📁 Proje İçerikleri

### 1. [PA1: Uçuş Gecikmeleri & Foodpanda SQL Analizi](./214-1)
* **Kapsam:** 
  * **Part 1 (Pandas EDA):** ABD Ulaştırma Bakanlığı'na ait uçuş ve hava durumu verileri (`flights.csv`, `flights_weather.csv`) birleştirilerek kalkış gecikmeleri, uçuş iptalleri, yağış ve rüzgar hızı faktörlerinin gecikme süreleri üzerindeki etkileri incelendi.
  * **Part 2 (SQLite & SQL):** `Foodpanda Analysis Dataset.csv` verisi için ilişkisel veri tabanı şeması (`Customers`, `Restaurants`, `Orders`) tasarlandı; `sqlite3` kullanılarak ciro, en çok satan yemek kategorileri, müşteri harcamaları, iptal/teslimat durumları ve şehir bazlı gelir dağılımları SQL sorgularıyla analiz edildi.
* **Kullanılan Teknolojiler:** `pandas`, `sqlite3`

---

### 2. [PA2: Superstore Perakende SQL Mimarisi & Netflix Trend Analizi](./214-2)
* **Kapsam:**
  * **Part 1 (İlişkisel Veri Tabanı Modellemesi):** `Sample - Superstore.csv` verisi 3NF yapısına uygun olarak `Customers`, `Products`, `Orders`, `OrderDetails` ve `Location` tablolarına ayrıştırıldı. Bellek içi (in-memory) SQLite üzerinde en karlı ürünler, müşteri segmenti performansları (Home Office vs. Corporate), coğrafi/kategori bazlı satış kırılımları ve birlikte en sık satın alınan ürün çiftleri (Market Basket Analysis) SQL ile analiz edildi.
  * **Part 2 (Veri Görselleştirme):** `netflix_titles.csv` veri seti üzerinden içerik türü dağılımı (Film vs. Dizi), yıllara göre içerik ekleme trendleri, popüler türler (Genres) ve en çok üretim yapan ilk 10 ülkenin dağılımı grafiklerle görselleştirildi.
* **Kullanılan Teknolojiler:** `pandas`, `sqlite3`, `numpy`, `matplotlib`

---

### 3. [PA3: Pırlanta Fiyat Tahmini ve Regresyon](./214-3)
* **Kapsam:**
  * **Keşifçi Veri Analizi:** ~54.000 pırlantaya ait fiziksel ve kalite öznitelikleri (`carat`, `cut`, `color`, `clarity`, `depth`, `table`, `x, y, z`) ile fiyat (`price`) arasındaki korelasyonlar ısı haritası (heatmap) ve saçılım grafikleriyle incelendi.
  * **Veri Ön İşleme:** Kategorik değişkenler için sıralı kodlama (Ordinal Encoding), eksik ve aykırı değer temizliği, özellik ölçekleme (StandardScaler/MinMaxScaler) adımları uygulandı.
  * **Model Eğitimi & Değerlendirme:** Pırlanta fiyatlarını tahmin etmek üzere doğrusal ve doğrusal olmayan regresyon modelleri eğitildi; model başarıları $R^2$, RMSE ve MAE metrikleriyle karşılaştırıldı.
* **Kullanılan Teknolojiler:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

### 4. [PA4: Havayolu Yolcu Memnuniyeti Sınıflandırması & Ülke Kümeleme](./214-4)
* **Kapsam:**
  * **Part 1 (Sınıflandırma):** `train.csv` havayolu yolcu verisi üzerinde ön işleme (One-Hot / Label Encoding, medyan/mod ile eksik veri tamamlama, standardizasyon) yapıldı. Veri kütüphanesiz (numpy ile rastgele) %80 eğitim - %20 test olarak ayrıldı. **Logistic Regression**, **kNN** ve **Decision Tree** modelleri eğitilip Doğruluk (Accuracy), Precision, Recall, F1-Score ve Karmaşıklık Matrisi (Confusion Matrix) metrikleriyle kıyaslandı. Lojistik regresyon katsayıları üzerinden memnuniyeti en çok etkileyen özellikler (Feature Importance) belirlendi.
  * **Part 2 (Kümeleme - Unsupervised Learning):** `country_data.csv` sosyo-ekonomik ve sağlık göstergeleri (çocuk ölümü, kişi başına gelir, yaşam beklentisi, enflasyon vb.) kullanılarak ülkelerin gelişmişlik düzeylerine göre kümelenmesi ve insani yardım önceliklendirmesi gerçekleştirildi.
* **Kullanılan Teknolojiler:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 🛠 Kullanılan Teknolojiler ve Kütüphaneler

* **Programlama Dili:** Python 3.x
* **Veri İşleme & SQL:** Pandas, NumPy, SQLite (`sqlite3`)
* **Makine Öğrenmesi:** Scikit-learn (Logistic Regression, k-Nearest Neighbors, Decision Trees, Regresyon Modelleri, Veri Ölçekleme)
* **Görselleştirme:** Matplotlib, Seaborn
* **Geliştirme Ortamı:** Jupyter Notebook
