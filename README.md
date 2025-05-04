# NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme

## 1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır.  
Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.

## 2. Kullanılan Veri Seti
- **Kaynak**: [AI Detection Student Writing (GitHub)](https://github.com)  
- **Boyut**: 1 dosya, CSV formatında, 22.1 MB  
- **Açıklama**: Her satır bir öğrenci ödevini temsil eder.

**Örnek Satır**:
```
Apply to 06_similarit...
```

## 3. Proje Klasör Yapısı
```
Apply to 06_similarit...
```

## 4. Kurulum ve Gerekli Kütüphaneler

Aşağıdaki Python kütüphaneleri gereklidir:

- pandas  
- numpy  
- nltk  
- gensim  
- scikit-learn  
- matplotlib  
- seaborn  

### Kurulum:
```bash
pip install pandas numpy nltk gensim scikit-learn matplotlib seaborn
```

## 5. Adım Adım Kullanım

### 1. Veri İnceleme ve Örnekleme
- Veri setinin boyutu, formatı ve örnek satırı ekrana yazdırılır.

### 2. Zipf Yasası Analizi
- Ham, lemmatized ve stemmed veri için Zipf grafikleri oluşturulur.

### 3. Ön İşleme (Preprocessing)
- Stopword removal, tokenization, lowercasing, lemmatization, stemming ve özel karakter temizliği yapılır.

**Çıktılar**:
- `essays_lemmatized.csv`
- `essays_stemmed.csv`
- `sentences_lemmatized.csv`
- `sentences_stemmed.csv`

### 4. TF-IDF Vektörleştirme
- TF-IDF ile lemmatize ve stem yapılmış metinlerin vektörleştirilmesi sağlanır.

**Çıktılar**:
- `tfidf_lemmatized.csv`
- `tfidf_stemmed.csv`

### 5. Word2Vec Model Testi
- Mevcut modellerden (örneğin `lemmatized_model_cbow_window2_dim100.model`) seçilen bir kelime için en benzer 5 kelime yazdırılır.

**Not**: Model dosyaları boyut nedeniyle repoya eklenmemiştir, sadece test kodu paylaşılmıştır.

### 6. Benzerlik Analizi
- Cosine similarity matrisleri ve benzerlik dağılımı grafikleri oluşturulur.

### 7. Detaylı Raporlama
- Yüksek benzerlikli çiftler CSV dosyasına kaydedilir.
- Detaylı eşleşme raporu oluşturulur.

## 6. Model Çıktıları Hakkında

- Word2Vec model dosyaları (`.model`) boyut nedeniyle GitHub’a yüklenmemiştir.
- Modelleri yeniden üretmek için preprocessing ve model eğitim kodları kullanılabilir.
- Model test kodları (örneğin `05_word2vec_training.py`) ile örnek kelime benzerlikleri alınabilir.

## 7. Veri Setinin Kullanım Amacı

- Öğrenci ödevlerinde intihal tespiti  
- Metin benzerliği analizi  
- Doğal dil işleme uygulamaları

Proje kapsamında metinlerin temizlenmesi, vektörleştirilmesi ve benzerliklerinin ölçülmesi örneklenmiştir.

## 8. Ek Bilgiler

- Tüm kodlar ve analizler `nlp.ipynb` dosyasında adım adım açıklanmıştır.
- PDF raporunda, kod çıktıları ve analizler detaylı şekilde sunulmuştur.
- Her adımda kullanılan kütüphaneler ve fonksiyonlar kod bloklarında belirtilmiştir.

## 9. Lisans

Bu proje eğitim amaçlıdır.
