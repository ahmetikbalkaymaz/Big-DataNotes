# Big Data Notes

### Büyük Veri Nedir ? 

Büyük Veri: Geleneksel yöntemlerle işlenemeyen verilere denir.

- Geleneksel yöntemlerle işlenememe durumu bazen verinin boyutu, bazen verinin türü bazen de verinin hızlı bir değişebiliyor olmasıdır.
- Bu problemin çözümü birden fazla bilgisayarın bir araya gelerek tek bir bilgisayar gibi hareket etmesidir. (Cluster Yapı)

### Büyük Verinin Bileşenleri

- Ortaya çıkan veri işleme güçlüğü verinin hacmi, çeşitliliği ve hızı ile alakalıdır.
- Büyük veriyi ifade eden özellikler hacim, çeşitlilik ve hızdır.

![bigdata3v (1)](https://user-images.githubusercontent.com/65342103/182160847-e588061d-cac7-4ffb-b176-feda2e8eb75d.png)

### Apache Hadoop

- Büyük veri teknolojisinin temelini oluşturur.
- Geleneksel yöntemler ile işlenmesi mümkün olmayan verilerin işlenmesine olanak sağlamaktadır.
- Bir bilgisayar kümesinin belirli bir işi yapmak için tek bir bilgisayar gibi birlikte hareket etmesini sağlamaktadır.

**Hadoop Dağıtık Dosya Sistemi (HDFS) :** Yerel dosya sistemleri olan FAT32 ve NFTS gibi bir dosya sistemidir. Bu sistemlerden
Farkı büyük boyutlardaki veriyi dağıtık şekilde depolamaya ve kontrol etmeye imkan sağlamaktadır.

**Hadoop MapReduce :** Büyük veri dünyasının fonksiyonel anlamda temelini oluşturan bileşendir. Aynı anda dağıtık bilgisayar 
kümeleri üzerinde büyük veri analizi yapılabilmesi için geliştirilmiş bir programlama modelidir.


### MapReduce Nedir?

<img width="350" alt="mapReduce" src="https://user-images.githubusercontent.com/65342103/182592916-513bfe27-2957-4ca3-8a85-5f1714ba73fd.png">

Map Aşamasının görevi, HDFS üzerindeki girdi verileri işlemektir.

Shuffle ve Reduce aşamalarının görevi, Map aşamasından gelen veriyi işlemek ve indirgemektir.

### Apache Hadoop Faydaları

- Veri saklama ve işlem gücü
- Açık Kaynak
- Hız
- Esneklik 
- Ölçeklenebilirlik
- Hata Toleransı


	• Disk tabanlı çalışan bir modeldir.
  
	• Her MapReduce görevinde diskten okuma ve diske yazma işlemi yapılır.
  
	• İteratif işlemler zaman alır ve kaynakları meşgul eder.
  
<img width="375" alt="diskbazlı" src="https://user-images.githubusercontent.com/65342103/182593670-aef9baa1-5ac3-4ee3-810d-a578dd06cad8.png">

### Apache Spark

Küme üzerinde hızlı ve genel amaçlı bilgi işleme sistemidir.

- Apache Hadoop'a göre 100 kat daha hızlı çalışmaktadır.
	
	### Apache Spark Bileşenleri
	
		- Spark Core ve RDD's
			• Hafıza Yönetimi
			• Görevlerin Dağıtılması
			• Hata Kurtarma
			• Dosya Sistemlerine Erişim
			• RDD's MapReduce'un alternatifidir.
			• Verinin bellek içi tutularak paralel işlenmesini ifade etmektedir.
		
		- Spark SQL
			• SQL ya da bir DataFrame API kullanarak Spark programlarında yapılandırılmış veriyi sorgulama imkanı sağlar
		
		- Spark MLlib
			• Ölçeklenebilir makine öğrenmesi kütüphanesidir.
		
		- Spark Streaming
			• Akan verinin ölçeklenebilir, yüksek hacimli ve hata toleranslı bir şekilde işlenmesine olanak sağlamaktadır.
	
		- GraphX
			• Paralel grafik tabanlı hesaplama işlemleri için kullanılan bir kütüphanedir.
### RDD's (Dayanıklı Dağıtık Data Setler)
RDD'de yapılan işlem veriyi RAM'e taşımak, RAM üzerinde dönüşüm işlemle
rini ve gerekli iteratif işlemleri yapmak ve en son işlemler
bittikten sonra veriyi tekrar diske yazmaktır.

### MapReduce ve RDD's Karşılaştırılması
<img width="450" alt="vs" src="https://user-images.githubusercontent.com/65342103/182594312-531eb613-556c-40e6-b773-fab8fafd0e1a.png">
