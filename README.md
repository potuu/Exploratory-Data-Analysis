# Exploratory-Data-Analysis
# Kaggle link:  https://www.kaggle.com/code/adilabdullayev/exploratory-data-analysis-on-bigbasket-dataset
# Ürün Fiyat ve Değerlendirmeleri Analizi

Bu proje, e-ticaret verilerini kullanarak ürünlerin fiyatları, kategorileri, markaları ve kullanıcı değerlendirmeleri hakkında derinlemesine bir analiz yapmayı amaçlamaktadır. Analiz, fiyat dağılımları, popüler markalar, kategorilere göre ortalama değerlendirmeler, indirim oranları ve daha pek çok metriği kapsamaktadır. Bu projede kullanılan Python kütüphaneleri arasında `pandas`, `matplotlib`, `seaborn` ve `wordcloud` yer almaktadır.

## Gerekli Kütüphaneler

- `pandas`: Veri işleme ve analiz için.
- `matplotlib`: Veri görselleştirme için.
- `seaborn`: Daha gelişmiş görselleştirmeler için.
- `wordcloud`: Ürün açıklamaları için kelime bulutları oluşturmak amacıyla.

## Veri Seti

Veri seti aşağıdaki sütunları içermektedir:

- `product`: Ürün adı
- `category`: Ürün kategorisi
- `sub_category`: Ürün alt kategorisi
- `brand`: Ürün markası
- `sale_price`: Ürün satış fiyatı
- `market_price`: Ürün piyasa fiyatı
- `type`: Ürün tipi
- `rating`: Ürün değerlendirme puanı
- `description`: Ürün açıklaması

## Analiz Adımları

### 1. **En Popüler Ürünlerin Görselleştirilmesi**
   - Ürünlerin satış sayılarına göre en popüler 10 ürünü bir pasta grafiği ile görselleştirilmiştir.

### 2. **Satış Fiyatı Dağılımı**
   - Ürünlerin satış fiyatlarının dağılımını görmek için histogram kullanılmıştır.

### 3. **Boxplot (Çeyrekler) Görselleştirmesi**
   - Satış fiyatlarının dağılımı ve aykırı değerler `boxplot` (çeyrekler) ile görselleştirilmiştir.

### 4. **İki Değişkenli İlişkiler**
   - **Fiyat ve Değerlendirme İlişkisi**: Ürünlerin satış fiyatı ile değerlendirme puanları arasındaki ilişki incelenmiştir.
   - **Fiyat ve İndirim Oranı İlişkisi**: Ürünlerin fiyatları ile indirim oranları arasındaki ilişki bir scatter plot ile gösterilmiştir.

### 5. **Kategorilere Göre Fiyat ve Rating Dağılımı**
   - Kategorilere göre ortalama fiyatlar ve ratingler görselleştirilmiştir. Ayrıca kategorilere göre ortalama indirim oranları da analiz edilmiştir.

### 6. **Marka Analizi**
   - En popüler 5 markanın satış fiyatları ve piyasa fiyatları boxplot ile görselleştirilmiştir.

### 7. **İndirimli Ürünlerin Performansı**
   - İndirimli ürünlerin değerlendirme puanları analiz edilmiştir. İndirimli ürünlerin ortalama değerlendirme puanı hesaplanmıştır.

### 8. **Aykırı Değerlerin Tespiti (IQR Yöntemi)**
   - Fiyat ve değerlendirme verileri için aykırı değerler (outliers) tespit edilmiştir. Bu işlem için IQR (Interquartile Range) kullanılmıştır.

### 9. **Kelime Frekansı Analizi**
   - Ürün açıklamaları üzerinden kelime bulutu (WordCloud) oluşturulmuştur. Bu, ürün açıklamalarındaki en sık geçen kelimeleri görselleştirir.

### 10. **Fiyat Segmentlerine Göre Rating Dağılımı**
   - Fiyat segmentlerine göre ortalama rating değerleri hesaplanarak görselleştirilmiştir.

## Kullanılan Yöntemler ve Teknikler

1. **Pandas DataFrame İşlemleri**:
   - Veri setindeki eksik değerler, aykırı değerler ve gruplama işlemleri için pandas kullanılmıştır.
   
2. **Matplotlib ve Seaborn**:
   - Farklı grafik türleri (bar chart, pie chart, scatter plot, boxplot, vs.) ile verinin görselleştirilmesi sağlanmıştır.
   
3. **İstatistiksel Yöntemler**:
   - Aykırı değerler için IQR yöntemi uygulanmıştır.
   - Satış fiyatı ve değerlendirme puanı arasındaki ilişki Pearson korelasyon katsayısı ile ölçülmüştür.

4. **Kelime Bulutu (WordCloud)**:
   - Ürün açıklamalarından kelime frekansı çıkarılarak görsel bir analiz yapılmıştır.

## Sonuçlar

- **Fiyat Dağılımı**: Ürünlerin çoğunluğu 0 ile 1000 arasında fiyatlandırılmıştır.
- **İndirimli Ürünlerin Performansı**: İndirimli ürünlerin ortalama değerlendirme puanı 3.94'tür.
- **Aykırı Değerler**: Fiyat ve değerlendirme verilerinde aykırı değerler tespit edilmiştir.
- **Kategorilere Göre Değerlendirme**: Bebek Bakımı kategorisi, ortalama olarak en yüksek fiyatlara sahipken, bazı kategorilerde indirim oranları da yüksek olmuştur.

## Görselleştirmeler

- **Pasta Grafikleri**: Popüler ürünlerin kategorilere göre dağılımı.
- **Bar Grafikleri**: Kategoriler ve markalar bazında fiyat ve değerlendirme puanlarının dağılımı.
- **Boxplot**: Fiyat ve değerlendirme puanlarının yayılımı.
- **WordCloud**: Ürün açıklamalarındaki kelime sıklıkları.

## Yorumlar

Bu analiz, e-ticaret platformlarında yer alan ürünler hakkında derinlemesine bir anlayış sağlar. Özellikle fiyat ve değerlendirme arasındaki ilişkiyi anlamak, müşterilerin ne tür ürünleri daha çok tercih ettiğini ve hangi fiyat aralıklarının daha popüler olduğunu gösterir.
