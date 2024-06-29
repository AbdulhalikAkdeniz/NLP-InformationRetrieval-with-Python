# NLP Information Retrieval with Cranfield Dataset

Bu proje, Cranfield veri seti kullanarak doğal dil işleme (NLP) ve bilgi erişimi (Information Retrieval) tekniklerini uygulamaktadır. 
Belgelerin ön işlenmesi, ters indeks oluşturma, boole sorguları ve TF-IDF hesaplama gibi adımları içermektedir.

- **Belgelerin ön işlenmesi**: Metinlerin küçük harfe dönüştürülmesi, tokenizasyon, stop words'lerin çıkarılması, normalizasyon ve kök bulma (Porter Stemmer) gibi adımları içerir.
- **Ters indeks oluşturma**: Belge koleksiyonundaki terimlerin sıklığını ve belge frekansını hesaplayarak ters indeks oluşturur.
- **Boole sorguları**: Kullanıcıların sorgularını Boole mantığı operatörleri (AND ve OR) ile işleyerek belge koleksiyonundan ilgili belgeleri bulmayı sağlar. OR sorgusu, herhangi bir terimin geçtiği belgeleri bulurken, AND sorgusu ise tüm terimleri içeren belgeleri bulur. 
- **TF-IDF tabanlı retrieval**: Belge ve sorgu vektörlerinin TF-IDF skorları üzerinden kosinüs benzerliği hesaplayarak en ilişkili belgeleri geri döndürür.

## Gereksinimler
Projeyi çalıştırmak için aşağıdaki Python kütüphanelerine ihtiyacınız olacak:

- nltk
- numpy
- pandas
- texttable

Bu kütüphaneleri yüklemek için aşağıdaki komutu kullanabilirsiniz:

```sh
pip install nltk numpy pandas texttable
```

## 📁 Proje Yapısı
**Information_Retrieval_with_Cranfield.ipynb**: Tüm kodların ve adımların bulunduğu Jupyter Notebook dosyası.

**cran.all.1400**: Cranfield koleksiyonundaki belgeleri içerir. Her belge bir kimlikle tanımlanır ve bilgi erişimi görevleri için metin verisi içerir.

**cran.qry**: Cranfield koleksiyonundaki sorguları içerir. Her sorgu bir kimlikle (ID) tanımlanır ve kullanıcıların belge koleksiyonunda arayabileceği metin içerir.

**cranqrel** : Bu Her bir sorgunun ilgili belgelere göre ilgi düzeyini gösteren değerlendirmeleri içerir. Bilgi erişim sistemlerinin performansını değerlendirmek için sorgu-belge ilgi düzeyi için gerçek veri sağlar.


## 🚀 Kullanım
- Jupyter Notebook dosyasını açın: `Information_Retrieval_with_Cranfield.ipynb`

- Her hücreyi sırayla çalıştırarak çıktıları inceleyin.

- NLTK veri dosyalarını indirmek için 
  ~~~
  nltk.download('punkt')
  ~~~
  ~~~
  nltk.download('stopwords')
  ~~~
   komutları çalıştırılmalıdır.

## Sonuçlar

**AND Query**

<img src="https://github.com/AbdulhalikAkdeniz/NLP-InformationRetrieval-with-Python/assets/139945380/a40d0bb1-40ea-45a5-ac4e-007a26713b94" alt="boolean" width="800"/>
 
 
 
**Cosine Similarity**

<img src="https://github.com/AbdulhalikAkdeniz/NLP-InformationRetrieval-with-Python/assets/139945380/6f5dc3e8-9546-4cfc-9fbb-3dd1202bba9d" alt="tfidf" width="800"/>



## Veri Seti
Bu projede Cranfield veri seti kullanılmıştır:

https://ir.dcs.gla.ac.uk/resources/test_collections/cran/

## 📧 İletişim
Sorularınız veya geri bildirimleriniz için, abdulhalikakdeniz08@gmail.com adresinden bana ulaşabilirsiniz.
