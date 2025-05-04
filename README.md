# NLP
NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme
1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır. Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.
2. Kullanılan Veri Seti
Kaynak: AI Detection Student Writing (GitHub)
Boyut: 1 dosya, CSV formatında, 22,1 MB
Açıklama: Her satır bir öğrenci ödevini temsil eder.
Örnek Satır:
Apply to 06_similarit...
3. Proje Klasör Yapısı
Apply to 06_similarit...
4. Kurulum ve Gerekli Kütüphaneler
Aşağıdaki kütüphaneler gereklidir:
pandas
numpy
nltk
gensim
scikit-learn
matplotlib
seaborn
Kurulum:
Apply to 06_similarit...
Run
5. Adım Adım Kullanım
1. Veri İnceleme ve Örnekleme
Apply to 06_similarit...
Run
Veri setinin boyutu, formatı ve örnek satırı ekrana yazdırılır.
2. Zipf Yasası Analizi
Apply to 06_similarit...
Run
Ham, lemmatized ve stemmed veri için Zipf grafikleri oluşturulur.
3. Ön İşleme (Preprocessing)
Apply to 06_similarit...
Run
Stopword removal, tokenization, lowercasing, lemmatization, stemming ve özel karakter temizliği yapılır.
Çıktılar: essays_lemmatized.csv, essays_stemmed.csv, sentences_lemmatized.csv, sentences_stemmed.csv
4. TF-IDF Vektörleştirme
Apply to 06_similarit...
Run
Çıktılar: tfidf_lemmatized.csv, tfidf_stemmed.csv
5. Word2Vec Model Testi
Apply to 06_similarit...
Run
Mevcut modellerden (ör: lemmatized_model_cbow_window2_dim100.model) seçilen bir kelime için en benzer 5 kelime ekrana yazdırılır.
Not: Model dosyaları boyut nedeniyle repoya eklenmemiştir, sadece test kodu paylaşılmıştır.
6. Benzerlik Analizi
Apply to 06_similarit...
Run
Cosine similarity matrisleri ve benzerlik dağılımı grafikleri oluşturulur.
7. Detaylı Raporlama
Apply to 06_similarit...
Run
Yüksek benzerlikli çiftler ve detaylı eşleşme raporu CSV olarak kaydedilir.
6. Model Çıktıları Hakkında
Word2Vec model dosyaları (ör: .model uzantılı) boyut nedeniyle GitHub’a yüklenmemiştir.
Modelleri yeniden üretmek için preprocessing ve model eğitim kodlarını kullanabilirsiniz.
Model test kodları (ör: 05_word2vec_training.py) ile mevcut modeller üzerinde örnek kelime benzerlikleri alınabilir.
7. Veri Setinin Kullanım Amacı
Bu veri seti, öğrenci ödevlerinde intihal tespiti, metin benzerliği analizi ve doğal dil işleme uygulamaları için kullanılabilir.
Proje kapsamında, metinlerin temizlenmesi, vektörleştirilmesi ve benzerliklerinin ölçülmesi adımları örneklenmiştir.
8. Ek Bilgiler
Tüm kodlar ve analizler nlp.ipynb dosyasında adım adım açıklanmıştır.
PDF raporunda, kod çıktıları ve analizler detaylı şekilde sunulmuştur.
Her adımda kullanılan kütüphaneler ve fonksiyonlar kod bloklarında belirtilmiştir.
9. Lisans
Bu proje eğitim amaçlıdır.
