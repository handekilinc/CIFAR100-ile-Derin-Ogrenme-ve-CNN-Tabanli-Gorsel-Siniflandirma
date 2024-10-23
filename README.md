# CIFAR-100 ile Derin Öğrenme ve CNN Tabanlı Görsel Sınıflandırma

## Hakkında
Bu proje, CIFAR-100 veri seti kullanılarak derin öğrenme teknikleri ile görsel sınıflandırma yeteneklerinin geliştirilmesine yönelik bir çalışmadır. Model, veri artırma yöntemleri ve hiperparametre optimizasyonu ile desteklenerek, görsel sınıflandırma problemlerine etkili çözümler sunmayı hedefler. CIFAR-100, CIFAR-10’a kıyasla daha karmaşık ve zengin sınıf yapısı sunarak, derin öğrenme uygulamalarının potansiyelini artırmaktadır.

## Proje Amacı
Projenin amacı, CIFAR-100 veri setini kullanarak derin öğrenme teknikleri ile görsel sınıflandırma modellerinin doğruluğunu artırmak ve bu modellerin gerçek dünya uygulamalarındaki etkinliğini test etmektir. Aynı zamanda, kullanılan çeşitli veri artırma ve model optimizasyon teknikleri sayesinde, sınıflandırma sonuçlarının güvenilirliğini ve genel performansını artırmayı hedefliyoruz.

## CIFAR-100 Veri Seti
CIFAR-100, 60,000 renkli görüntüden oluşan ve 100 farklı sınıfa ait 32x32 piksel boyutunda küçük resimlerden oluşan bir veri setidir. Veri seti, 20 aileye ayrılmıştır ve her aile 5 sınıf içerir. Örneğin, "hayvanlar" ailesi "kedi", "köpek", "kuş", "sığır" ve "at" gibi sınıfları içerir. CIFAR-100, görsel sınıflandırma ve derin öğrenme alanında yaygın olarak kullanılan bir veri setidir ve daha karmaşık yapısıyla model geliştirmeleri için zorlu bir zemin sunar. 

## CIFAR-100 Veri Seti Hakkında

CIFAR-100 veri seti, CIFAR-10 ile benzerlik göstermektedir; ancak 100 sınıf içermektedir ve her sınıfta 600 görsel bulunmaktadır. Her sınıf için 500 eğitim görseli ve 100 test görseli mevcuttur. CIFAR-100'deki 100 sınıf, 20 süper sınıf altında gruplandırılmıştır. Her görüntü, "ince" etiket (ait olduğu sınıf) ve "kabaca" etiket (ait olduğu süper sınıf) ile birlikte gelir.

### CIFAR-100 Sınıfları
- **Süper Sınıf 1**
  - Sınıf 1
  - Sınıf 2
  - Sınıf 3
  - ...
- **Süper Sınıf 2**
  - Sınıf 1
  - Sınıf 2
  - Sınıf 3
  - ...
- ...
- **Süper Sınıf 20**
  - Sınıf 1
  - Sınıf 2
  - Sınıf 3
  - ...

## CIFAR-100 Süper Sınıflar ve Sınıflar

| Süper Sınıf                           | Sınıflar                                                      |
|---------------------------------------|--------------------------------------------------------------|
| **Aquatic Mammals**                  | beaver, dolphin, otter, seal, whale                         |
| **Fish**                              | aquarium fish, flatfish, ray, shark, trout                  |
| **Flowers**                           | orchids, poppies, roses, sunflowers, tulips                 |
| **Food Containers**                   | bottles, bowls, cans, cups, plates                           |
| **Fruit and Vegetables**              | apples, mushrooms, oranges, pears, sweet peppers             |
| **Household Electrical Devices**      | clock, computer keyboard, lamp, telephone, television        |
| **Household Furniture**                | bed, chair, couch, table, wardrobe                           |
| **Insects**                           | bee, beetle, butterfly, caterpillar, cockroach              |
| **Large Carnivores**                 | bear, leopard, lion, tiger, wolf                             |
| **Large Man-Made Outdoor Things**    | bridge, castle, house, road, skyscraper                      |
| **Large Natural Outdoor Scenes**      | cloud, forest, mountain, plain, sea                          |
| **Large Omnivores and Herbivores**   | camel, cattle, chimpanzee, elephant, kangaroo               |
| **Medium-Sized Mammals**             | fox, porcupine, possum, raccoon, skunk                      |
| **Non-Insect Invertebrates**         | crab, lobster, snail, spider, worm                           |
| **People**                            | baby, boy, girl, man, woman                                 |
| **Reptiles**                         | crocodile, dinosaur, lizard, snake, turtle                  |
| **Small Mammals**                    | hamster, mouse, rabbit, shrew, squirrel                     |
| **Trees**                            | maple, oak, palm, pine, willow                               |
| **Vehicles 1**                       | bicycle, bus, motorcycle, pickup truck, train                |
| **Vehicles 2**                       | lawn-mower, rocket, streetcar, tank, tractor                 |



## Kullanım Alanları
Bu proje, geniş bir uygulama yelpazesine sahiptir:
- **Otomatik Görüntü Etiketleme**: Büyük veri havuzlarındaki görsellerin hızlı bir şekilde sınıflandırılmasına olanak tanır.
- **Oyun Geliştirme**: Görsel tanıma sistemleri ile oyunlarda karakter veya nesnelerin tanınması ve etkileşimli deneyimlerin oluşturulması.
- **Reklamcılık ve Pazarlama**: Kullanıcı davranışlarını anlamak için görsel içerik analizi yaparak hedefli reklam kampanyalarının oluşturulmasına yardımcı olur.
- **Güvenlik Sistemleri**: Tehditleri tanımlamak için görüntü sınıflandırma sistemlerinin entegrasyonu, güvenlik önlemlerinin artırılmasına yardımcı olabilir.
- **Tıp ve Sağlık**: Görüntü analizi ile hastalıkların erken teşhisi ve tedavi süreçlerinde destek sağlama.
- **Otonom Araçlar**: Görsel tanıma ile çevresel algılama ve otomatik navigasyon sistemlerinin geliştirilmesi.

## Kullanılan Kütüphaneler
Bu projede kullanılan başlıca kütüphaneler şunlardır:
- **TensorFlow**: Derin öğrenme modellerinin geliştirilmesi için kullanılan açık kaynak kütüphanesi.
- **Keras**: TensorFlow üzerinde çalışan, hızlı prototipleme ve model geliştirme için idealdir.
- **NumPy**: Sayısal veri işlemleri ve matris hesaplamaları için kullanılan güçlü bir kütüphane.
- **Matplotlib**: Veri görselleştirme amacıyla kullanılan kütüphane, grafiklerin oluşturulmasını sağlar.
- **Scikit-learn**: Hiperparametre optimizasyonu ve veri ön işleme için kullanılan kapsamlı bir kütüphane.

## CNN Tanımı ve Kullanım Nedeni
**Konvolüsyonel Sinir Ağı (CNN)**, görüntü işleme görevlerinde yüksek performans gösteren bir derin öğrenme mimarisidir. CNN'ler, görüntülerdeki temel özellikleri otomatik olarak öğrenme yeteneğine sahip olduğu için, sınıflandırma görevlerinde oldukça etkilidir. Bu projede CNN kullanmamızın birkaç nedeni şunlardır:
- **Özellik Öğrenme**: CNN, görüntülerdeki temel özellikleri (kenarlar, dokular vb.) otomatik olarak öğrenerek daha etkili bir sınıflandırma yapabilir.
- **Parametre Paylaşımı**: CNN'ler, ağırlıkları paylaştıkları için daha az parametre ile çalışarak daha hızlı ve etkili öğrenme sağlar.
- **Havuzlama (Pooling)**: CNN'ler, havuzlama katmanları kullanarak özellikleri sıkıştırabilir ve modelin genel doğruluğunu artırabilir.

## Gelecekteki Araştırmalar
Gelecekteki araştırmalara dair öneriler şunlardır:
1. **Gelişmiş Veri Artırma Teknikleri**: Görüntü verileri üzerinde daha karmaşık artırma tekniklerinin uygulanması, örneğin:
   - **Renk Değişiklikleri**: Görüntülerin renk doygunluğunun veya tonlarının değiştirilmesi.
   - **Kontrast Ayarları**: Görüntülerin kontrast değerlerinin ayarlanması ile daha fazla görsel çeşitlilik sağlanması.
   - **Gaussian Gürültüsü**: Görüntülere rastgele gürültü ekleyerek modelin genel dayanıklılığının artırılması.
   - **Dönme ve Çevirme**: Görüntülerin belirli açılarda döndürülmesi veya yatay/dikey olarak çevrilmesi, modelin farklı görünümleri tanıma yeteneğini artırabilir.

2. **Transfer Öğrenimi**: Önceden eğitilmiş modellerin kullanımı ile daha az veri ile yüksek performans elde edilmesi, böylece sınırlı veri setleri ile çalışırken verimliliğin artırılması.

3. **Gerçek Zamanlı Uygulamalar**: Modelin gerçek zamanlı veri akışları üzerinde çalıştırılması, akıllı uygulamalar ve otomatik tanıma sistemleri geliştirme potansiyelini artırır.

4. **Modeli İnce Ayar Yapma**: Daha derin ve karmaşık modellerin tasarlanması, farklı ağ mimarileri ile deneyler yaparak sonuçların iyileştirilmesi.

## Sonuçlar ve Değerlendirme
Proje sonucunda, CIFAR-100 veri seti üzerinde geliştirilen derin öğrenme modelinin başarısı önemli ölçüde artmıştır. Uygulanan veri artırma ile modelin doğruluğu %80’in üzerine çıkmıştır. Eğitim sürecinin ardından elde edilen doğruluk ve kayıp grafiklerinin görselleştirilmesi, modelin öğrenme sürecini daha iyi anlamamıza olanak tanımıştır. 

### Sonuçların Değerlendirilmesi
Elde edilen sonuçlar, modelin genel doğruluğunun artışını ve eğitim sürecinin etkinliğini göstermektedir. Doğruluk grafiği, modelin her eğitim epoch'unda performansını artırdığını ortaya koymakta, kayıp grafiği ise modelin öğrenme sürecindeki iyileşmeleri göstermektedir. Ek olarak, modelin overfitting (aşırı öğrenme) sorununu önlemek için uygulanan veri artırma tekniklerinin etkili olduğu gözlemlenmiştir. 

Sonuç olarak, CIFAR-100 veri setindeki daha karmaşık yapılar ve sınıflar sayesinde, geliştirilen modelin görsel sınıflandırma yeteneklerinin daha da ileriye taşınması mümkün olmuştur. Gelecekte yapılacak çalışmalar, bu alandaki yenilikçi uygulamaları destekleyecek ve derin öğrenme alanındaki gelişmelere katkı sağlayacaktır.

## Kullanılan Adımlar
1. **Veri Setini Yükleme**: CIFAR-100 veri setinin indirilmesi ve yüklenmesi.
2. **Veri Ön İşleme**: Verilerin normalizasyonu ve eğitim/test setlerine ayrılması.
3. **Veri Artırma**: Modelin genel dayanıklılığını artırmak için veri artırma tekniklerinin uygulanması.
4. **Modelin Oluşturulması**: CNN mimarisinin tasarlanması ve oluşturulması.
5. **Modelin Eğitilmesi**: Eğitim sürecinin başlatılması ve modelin eğitilmesi.
6. **Modelin Değerlendirilmesi**: Doğruluk ve kayıp grafiklerinin oluşturulması.
7. **Sonuçların Görselleştirilmesi**: Modelin öğrenme sürecinin grafiklerle sunulması.
