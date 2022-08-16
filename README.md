# Veri Seti
 Veri seti 4242 çiçek resmi içermektedir. Resimler beş sınıfa ayrılmıştır: papatya, lale, gül, ayçiçeği ve karahindiba. Her sınıf için yaklaşık 800 fotoğraf var ve veriler %80 train , %20 test olarak ayrılmış.
![image](https://user-images.githubusercontent.com/96024765/184877171-0100b471-f8dc-42b6-a0be-80e1ebca29b7.png)

# Modeller
# 1)AlexNet
İlk beş tanesi konvolüsyonel, son üç tanesi ise tam bağlı katman olan sekiz katmandan oluşmaktadır. Bu katmanlar arasında “pooling” ve “aktivasyon” katmanları da bulunmaktadır. Başarıyı artırmak ve overfittingi önlemek için tam bağlı katmanların arasına iki tane dropout ekledim.

# 2)VggNet-19
Mimarisinde 3x3 konvolüsyon katmanlarından sonra max pooling katmanı, sonunda ise 3 adet Fully Connected (tam bağlı) katman barındırmaktadır. Başarıyı arttırmak için tam bağlı katmanların arasına iki tane dropout ekledim. VGG'nin en büyük katkısı derinliğin sınıflandırmada önemini göstermesidir.

# 3)ResNet-50
ResNet50 evrişimsel sinir ağı genel olarak; konvolüsyon katmanı, aktivasyon katmanı, pooling katmanı ve tam bağlı katman gruplarından meydana gelmektedir. Başarıyı arttırabilmek için tam bağlı katmanların arasına 3 tane batch_normalization ekledim.

# Modellerin Test Edilmesi
![image](https://user-images.githubusercontent.com/96024765/184877595-4a0d4d01-cf34-4040-9a0d-1eddbc6c6d34.png)
![image](https://user-images.githubusercontent.com/96024765/184877629-db234e75-030d-4270-adea-e05cea343f82.png)

# Sonuçlar
![image](https://user-images.githubusercontent.com/96024765/184877783-55e1deda-2513-4b3b-aa33-eb57af3c81f9.png)
Sonuçlar değerlendirildikten sonra en yüksek başarıya ulaşan model %73,14 ile VGGNet-16 modeli olmuştur.





