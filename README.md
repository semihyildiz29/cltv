CUSTOMER LIFETIME VALUE (Müşteri Yaşam Boyu Değeri)

Bu proje, müşteri yaşam boyu değerini (CLTV) hesaplamak için çeşitli analizler ve hesaplamalar yapmayı amaçlar. Proje, bir veri setini kullanarak müşteri değerini belirlemek ve segmentasyon yaparak iş kararlarını desteklemeyi hedefler.

İçindekiler
1. Veri Hazırlama
2. Average Order Value (Ortalama Sipariş Değeri)
3. Purchase Frequency (Satın Alma Sıklığı)
4. Repeat Rate & Churn Rate (Tekrar Oranı & Churn Oranı)
5. Profit Margin (Kar Marjı)
6. Customer Value (Müşteri Değeri)
7. Customer Lifetime Value (CLTV)
8. Segmentlerin Oluşturulması
9. BONUS: Tüm İşlemlerin Fonksiyonlaştırılması

Veri Seti

- Veri Seti: [Online Retail II](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)
- Açıklama: Online Retail II isimli veri seti, İngiltere merkezli online bir satış mağazasının 01/12/2009 - 09/12/2011 tarihleri arasındaki satışlarını içerir.

Değişkenler
- InvoiceNo: Fatura numarası. Her işleme yani faturaya ait eşsiz numara. "C" ile başlıyorsa iptal edilen işlem.
- StockCode: Ürün kodu. Her bir ürün için eşsiz numara.
- Description: Ürün ismi.
- Quantity: Ürün adedi. Faturalardaki ürünlerden kaçar tane satıldığını ifade eder.
- InvoiceDate: Fatura tarihi ve zamanı.
- UnitPrice: Ürün fiyatı (Sterlin cinsinden).
- CustomerID: Eşsiz müşteri numarası.
- Country: Ülke ismi. Müşterinin yaşadığı ülke.

Analiz Adımları

1. Veri Hazırlama
Veri setini temizleme ve analiz için hazırlama adımları.

2. Average Order Value (Ortalama Sipariş Değeri)
Ortalama sipariş değerini hesaplama: `average_order_value = total_price / total_transaction`.

3. Purchase Frequency (Satın Alma Sıklığı)
Satın alma sıklığını hesaplama: `purchase_frequency = total_transaction / total_number_of_customers`.

4. Repeat Rate & Churn Rate (Tekrar Oranı & Churn Oranı)
Birden fazla alışveriş yapan müşteri sayısının tüm müşterilere oranı ile churn oranını hesaplama.

5. Profit Margin (Kar Marjı)
Kar marjını hesaplama: `profit_margin = total_price * 0.10`.

6. Customer Value (Müşteri Değeri)
Müşteri değerini hesaplama: `customer_value = average_order_value * purchase_frequency`.

7. Customer Lifetime Value (CLTV)
CLTV hesaplama: `CLTV = (customer_value / churn_rate) x profit_margin`.

8. Segmentlerin Oluşturulması
Müşterileri farklı segmentlere ayırma.

9. BONUS: Tüm İşlemlerin Fonksiyonlaştırılması
Analizlerin ve hesaplamaların fonksiyonlar halinde düzenlenmesi.

Katkıda Bulunma

Bu proje üzerinde geliştirme yapmak istiyorsanız, lütfen projeyi fork'layın ve pull request gönderin. Her türlü katkı kabul edilir.

Lisans

Bu proje MIT Lisansı altında lisanslanmıştır.
