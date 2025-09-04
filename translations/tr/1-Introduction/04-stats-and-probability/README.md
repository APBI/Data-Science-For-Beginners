<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "8bbb3fa0d4ad61384a3b4b5f7560226f",
  "translation_date": "2025-09-04T18:15:04+00:00",
  "source_file": "1-Introduction/04-stats-and-probability/README.md",
  "language_code": "tr"
}
-->
# İstatistik ve Olasılığa Kısa Bir Giriş

|![ Sketchnote by [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/04-Statistics-Probability.png)|
|:---:|
| İstatistik ve Olasılık - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

İstatistik ve Olasılık Teorisi, Matematiğin birbiriyle yakından ilişkili ve Veri Bilimi açısından oldukça önemli iki alanıdır. Matematik hakkında derin bir bilgiye sahip olmadan veriyle çalışmak mümkün olsa da, en azından bazı temel kavramları bilmek her zaman daha iyidir. Burada, başlangıç yapmanıza yardımcı olacak kısa bir giriş sunacağız.

[![Tanıtım Videosu](../../../../translated_images/video-prob-and-stats.e4282e5efa2f2543400843ed98b1057065c9600cebfc8a728e8931b5702b2ae4.tr.png)](https://youtu.be/Z5Zy85g4Yjw)

## [Ders Öncesi Testi](https://purple-hill-04aebfb03.1.azurestaticapps.net/quiz/6)

## Olasılık ve Rastgele Değişkenler

**Olasılık**, bir **olayın** ne kadar olası olduğunu ifade eden 0 ile 1 arasında bir sayıdır. Pozitif sonuçların (olaya yol açan sonuçlar) toplam sonuçlara bölünmesiyle tanımlanır, tüm sonuçların eşit olasılıkla gerçekleştiği varsayılır. Örneğin, bir zar attığımızda, çift sayı gelme olasılığı 3/6 = 0.5'tir.

Olaylardan bahsederken **rastgele değişkenler** kullanırız. Örneğin, bir zar attığımızda elde edilen sayıyı temsil eden rastgele değişken 1 ile 6 arasında değerler alır. 1'den 6'ya kadar olan sayı kümesine **örnek uzayı** denir. Rastgele bir değişkenin belirli bir değeri alma olasılığından bahsedebiliriz, örneğin P(X=3)=1/6.

Önceki örnekteki rastgele değişken **ayrık** olarak adlandırılır, çünkü sayılabilir bir örnek uzayına sahiptir, yani ayrı ayrı sıralanabilir değerler vardır. Örnek uzayının gerçek sayıların bir aralığı veya tüm gerçek sayı kümesi olduğu durumlar da vardır. Bu tür değişkenlere **sürekli** denir. İyi bir örnek, otobüsün varış zamanı olabilir.

## Olasılık Dağılımı

Ayrık rastgele değişkenler durumunda, her olayın olasılığını P(X) fonksiyonu ile tanımlamak kolaydır. Örnek uzayı *S*'den her bir *s* değeri için, 0 ile 1 arasında bir sayı verir ve tüm olaylar için P(X=s) değerlerinin toplamı 1 olur.

En bilinen ayrık dağılım **uniform dağılım**dır, burada N elemanlı bir örnek uzayı vardır ve her biri için eşit olasılık 1/N'dir.

Sürekli bir değişkenin olasılık dağılımını tanımlamak daha zordur, değerler [a,b] aralığından veya tüm gerçek sayı kümesi ℝ'den alınır. Otobüsün varış zamanı durumunu düşünün. Aslında, her bir kesin varış zamanı *t* için, otobüsün tam olarak o zamanda gelme olasılığı 0'dır!

> Şimdi biliyorsunuz ki olasılığı 0 olan olaylar gerçekleşir ve çok sık gerçekleşir! En azından her otobüs geldiğinde!

Sadece bir değişkenin belirli bir değer aralığına düşme olasılığından bahsedebiliriz, örneğin P(t<sub>1</sub>≤X<t<sub>2</sub>). Bu durumda, olasılık dağılımı **olasılık yoğunluk fonksiyonu** p(x) ile tanımlanır, böylece

![P(t_1\le X<t_2)=\int_{t_1}^{t_2}p(x)dx](../../../../translated_images/probability-density.a8aad29f17a14afb519b407c7b6edeb9f3f9aa5f69c9e6d9445f604e5f8a2bf7.tr.png)

Sürekli uniform dağılımın sürekli analoğu, sonlu bir aralıkta tanımlanır. X'in uzunluğu l olan bir aralığa düşme olasılığı l ile orantılıdır ve 1'e kadar yükselir.

Bir diğer önemli dağılım **normal dağılım**dır, aşağıda daha ayrıntılı olarak ele alacağız.

## Ortalama, Varyans ve Standart Sapma

Bir rastgele değişken X'in n örneğini alalım: x<sub>1</sub>, x<sub>2</sub>, ..., x<sub>n</sub>. **Ortalama** (veya **aritmetik ortalama**) değeri, geleneksel şekilde (x<sub>1</sub>+x<sub>2</sub>+x<sub>n</sub>)/n olarak tanımlanabilir. Örnek boyutunu büyüttükçe (yani n→∞ sınırını aldığımızda), dağılımın ortalamasını (aynı zamanda **beklenti** olarak adlandırılır) elde ederiz. Beklentiyi **E**(x) ile göstereceğiz.

> Herhangi bir ayrık dağılım için, {x<sub>1</sub>, x<sub>2</sub>, ..., x<sub>N</sub>} değerleri ve karşılık gelen olasılıklar p<sub>1</sub>, p<sub>2</sub>, ..., p<sub>N</sub> ile, beklenti E(X)=x<sub>1</sub>p<sub>1</sub>+x<sub>2</sub>p<sub>2</sub>+...+x<sub>N</sub>p<sub>N</sub> olur.

Değerlerin ne kadar yayıldığını belirlemek için varyansı hesaplayabiliriz: σ<sup>2</sup> = ∑(x<sub>i</sub> - μ)<sup>2</sup>/n, burada μ dizinin ortalamasıdır. σ değeri **standart sapma**, σ<sup>2</sup> ise **varyans** olarak adlandırılır.

## Mod, Medyan ve Çeyrekler

Bazen, ortalama veriler için "tipik" değeri yeterince temsil etmez. Örneğin, birkaç aşırı değer tamamen aralık dışındaysa, bunlar ortalamayı etkileyebilir. Bir diğer iyi gösterge **medyan**dır, verilerin yarısının altında, diğer yarısının üstünde olduğu bir değerdir.

Veri dağılımını anlamamıza yardımcı olmak için **çeyreklerden** bahsetmek faydalıdır:

* Birinci çeyrek, veya Q1, verilerin %25'inin altında olduğu bir değerdir
* Üçüncü çeyrek, veya Q3, verilerin %75'inin altında olduğu bir değerdir

Medyan ve çeyrekler arasındaki ilişkiyi grafiksel olarak **kutu grafiği** adı verilen bir diyagramda gösterebiliriz:

<img src="images/boxplot_explanation.png" width="50%"/>

Burada ayrıca **çeyrekler arası aralık** IQR=Q3-Q1 ve **aykırı değerler** - [Q1-1.5*IQR,Q3+1.5*IQR] sınırlarının dışında kalan değerler hesaplanır.

Küçük bir olası değerler kümesi içeren sonlu bir dağılım için, en sık görülen "tipik" değer **mod** olarak adlandırılır. Genellikle kategorik verilere uygulanır, örneğin renkler. İki grup insan olduğunu düşünün - bazıları kırmızıyı, diğerleri maviyi tercih ediyor. Renkleri sayılarla kodlarsak, favori renk için ortalama değer turuncu-yeşil spektrumunda bir yerde olur, bu da hiçbir grubun gerçek tercihini göstermez. Ancak mod, ya bir renk ya da her iki renk olur, eğer oy veren kişi sayısı eşitse (bu durumda örnek **çok modlu** olarak adlandırılır).

## Gerçek Dünya Verileri

Gerçek hayattan veri analiz ettiğimizde, genellikle bilinmeyen sonuçlarla deneyler yapmadığımız anlamda rastgele değişkenler değildirler. Örneğin, bir beyzbol takımı ve oyuncularının boy, kilo ve yaş gibi vücut verilerini düşünün. Bu sayılar tam olarak rastgele değildir, ancak yine de aynı matematiksel kavramları uygulayabiliriz. Örneğin, insanların ağırlıklarının bir dizisi, bir rastgele değişkenden alınan bir değerler dizisi olarak düşünülebilir. Aşağıda [Major League Baseball](http://mlb.mlb.com/index.jsp) oyuncularının ağırlıklarının dizisi verilmiştir, [bu veri setinden](http://wiki.stat.ucla.edu/socr/index.php/SOCR_Data_MLB_HeightsWeights) alınmıştır (kolaylık sağlamak için sadece ilk 20 değer gösterilmiştir):

```
[180.0, 215.0, 210.0, 210.0, 188.0, 176.0, 209.0, 200.0, 231.0, 180.0, 188.0, 180.0, 185.0, 160.0, 180.0, 185.0, 197.0, 189.0, 185.0, 219.0]
```

> **Not**: Bu veri setiyle çalışma örneğini görmek için [ilgili notebook](notebook.ipynb)'a göz atabilirsiniz. Bu ders boyunca bir dizi zorluk da bulunmaktadır ve bu notebook'a biraz kod ekleyerek tamamlayabilirsiniz. Veriler üzerinde nasıl işlem yapacağınızı bilmiyorsanız endişelenmeyin - Python kullanarak veri üzerinde çalışmaya daha sonra geri döneceğiz. Jupyter Notebook'ta kod çalıştırmayı bilmiyorsanız, [bu makaleye](https://soshnikov.com/education/how-to-execute-notebooks-from-github/) göz atabilirsiniz.

İşte verilerimiz için ortalama, medyan ve çeyrekleri gösteren kutu grafiği:

![Ağırlık Kutu Grafiği](../../../../translated_images/weight-boxplot.1dbab1c03af26f8a008fff4e17680082c8ab147d6df646cbac440bbf8f5b9c42.tr.png)

Verilerimiz farklı oyuncu **rolleri** hakkında bilgi içerdiğinden, rollere göre kutu grafiği de yapabiliriz - bu, parametre değerlerinin roller arasında nasıl farklılık gösterdiği hakkında fikir edinmemizi sağlar. Bu sefer boyu ele alacağız:

![Role göre kutu grafiği](../../../../translated_images/boxplot_byrole.036b27a1c3f52d42f66fba2324ec5cde0a1bca6a01a619eeb0ce7cd054b2527b.tr.png)

Bu diyagram, ortalama olarak birinci basemenlerin boyunun ikinci basemenlerin boyundan daha yüksek olduğunu göstermektedir. Bu dersin ilerleyen bölümlerinde bu hipotezi daha resmi bir şekilde nasıl test edebileceğimizi ve verilerimizin bunu göstermek için istatistiksel olarak anlamlı olduğunu nasıl kanıtlayabileceğimizi öğreneceğiz.

> Gerçek dünya verileriyle çalışırken, tüm veri noktalarının bir olasılık dağılımından alınan örnekler olduğunu varsayarız. Bu varsayım, makine öğrenimi tekniklerini uygulamamıza ve çalışan tahmin modelleri oluşturmamıza olanak tanır.

Verilerimizin dağılımını görmek için **histogram** adı verilen bir grafik çizebiliriz. X ekseni, farklı ağırlık aralıklarını (sözde **binler**) içerir ve dikey eksen, rastgele değişken örneğimizin belirli bir aralıkta olduğu zamanların sayısını gösterir.

![Gerçek dünya verilerinin histogramı](../../../../translated_images/weight-histogram.bfd00caf7fc30b145b21e862dba7def41c75635d5280de25d840dd7f0b00545e.tr.png)

Bu histogramdan, tüm değerlerin belirli bir ortalama ağırlık etrafında toplandığını ve bu ağırlıktan uzaklaştıkça o değerdeki ağırlıkların daha az sıklıkla karşılaşıldığını görebilirsiniz. Yani, bir beyzbol oyuncusunun ağırlığının ortalama ağırlıktan çok farklı olması çok olası değildir. Ağırlıkların varyansı, ağırlıkların ortalamadan ne kadar farklı olma olasılığını gösterir.

> Eğer beyzbol liginden olmayan diğer insanların ağırlıklarını alırsak, dağılım muhtemelen farklı olacaktır. Ancak, dağılımın şekli aynı kalacak, sadece ortalama ve varyans değişecektir. Bu nedenle, modelimizi beyzbol oyuncuları üzerinde eğitirsek, üniversite öğrencilerine uygulandığında yanlış sonuçlar vermesi muhtemeldir, çünkü temel dağılım farklıdır.

## Normal Dağılım

Yukarıda gördüğümüz ağırlık dağılımı çok tipiktir ve gerçek dünyadan birçok ölçüm aynı türde dağılımı takip eder, ancak farklı ortalama ve varyanslarla. Bu dağılıma **normal dağılım** denir ve istatistikte çok önemli bir rol oynar.

Normal dağılım kullanmak, potansiyel beyzbol oyuncularının rastgele ağırlıklarını üretmenin doğru bir yoludur. Bir kez `mean` (ortalama ağırlık) ve `std` (standart sapma) değerlerini bildiğimizde, 1000 ağırlık örneğini şu şekilde üretebiliriz:
```python
samples = np.random.normal(mean,std,1000)
``` 

Üretilen örneklerin histogramını çizersek, yukarıda gösterilen resme çok benzeyen bir görüntü göreceğiz. Örnek sayısını ve bin sayısını artırırsak, ideal bir normal dağılıma daha yakın bir görüntü oluşturabiliriz:

![Ortalama=0 ve std.dev=1 ile Normal Dağılım](../../../../translated_images/normal-histogram.dfae0d67c202137d552d0015fb87581eca263925e512404f3c12d8885315432e.tr.png)

*Ortalama=0 ve std.dev=1 ile Normal Dağılım*

## Güven Aralıkları

Beyzbol oyuncularının ağırlıklarından bahsederken, tüm beyzbol oyuncularının ağırlıklarının ideal olasılık dağılımına karşılık gelen **rastgele değişken W** olduğunu varsayarız (sözde **popülasyon**). Ağırlık dizimiz, **örnek** olarak adlandırdığımız tüm beyzbol oyuncularının bir alt kümesine karşılık gelir. İlginç bir soru şu: W'nin dağılım parametrelerini, yani popülasyonun ortalama ve varyansını bilebilir miyiz?

En kolay cevap, örneğimizin ortalama ve varyansını hesaplamak olacaktır. Ancak, rastgele örneğimizin tam popülasyonu doğru bir şekilde temsil etmediği durumlar olabilir. Bu nedenle **güven aralığı** hakkında konuşmak mantıklıdır.
> **Güven aralığı**, örneklemimize dayanarak popülasyonun gerçek ortalamasını tahmin etmemizi sağlar ve belirli bir olasılık (veya **güven düzeyi**) ile doğrudur.
Varsayalım ki dağılımımızdan X<sub>1</sub>, ..., X<sub>n</sub> örneklerini aldık. Dağılımımızdan her örnek aldığımızda, farklı bir ortalama değer μ elde ederiz. Bu nedenle μ bir rastgele değişken olarak düşünülebilir. Güven aralığı p güveniyle (L<sub>p</sub>,R<sub>p</sub>) değer çiftidir, öyle ki **P**(L<sub>p</sub>≤μ≤R<sub>p</sub>) = p, yani ölçülen ortalama değerin bu aralık içinde olma olasılığı p'ye eşittir.

Bu güven aralıklarının nasıl hesaplandığını detaylı bir şekilde tartışmak kısa girişimizin ötesine geçer. Daha fazla detayı [Wikipedia'da](https://en.wikipedia.org/wiki/Confidence_interval) bulabilirsiniz. Kısaca, hesaplanan örnek ortalamasının gerçek popülasyon ortalamasına göre dağılımını tanımlarız, bu dağılıma **student dağılımı** denir.

> **İlginç bir bilgi**: Student dağılımı, matematikçi William Sealy Gosset'in takma adı "Student" altında yayınladığı makalesinden adını almıştır. Gosset, Guinness bira fabrikasında çalışıyordu ve bir versiyona göre, işvereni, ham maddelerin kalitesini belirlemek için istatistiksel testler kullandıklarını genel halkın bilmesini istemiyordu.

Popülasyonumuzun ortalaması μ'yu p güveniyle tahmin etmek istiyorsak, bir Student dağılımı A'nın *(1-p)/2'nci yüzdelik dilimini* almamız gerekir. Bu değer tablolarından alınabilir veya istatistiksel yazılımın (örneğin Python, R, vb.) yerleşik fonksiyonları kullanılarak hesaplanabilir. Daha sonra μ için aralık X±A*D/√n olarak verilir, burada X örnekten elde edilen ortalama, D ise standart sapmadır.

> **Not**: Ayrıca [serbestlik dereceleri](https://en.wikipedia.org/wiki/Degrees_of_freedom_(statistics)) kavramını tartışmayı atlıyoruz, bu kavram Student dağılımı ile ilişkilidir. Bu kavramı daha derin anlamak için istatistik üzerine daha kapsamlı kitaplara başvurabilirsiniz.

Ağırlıklar ve boylar için güven aralığı hesaplama örneği [eşlik eden not defterinde](notebook.ipynb) verilmiştir.

| p | Ağırlık ortalaması |
|-----|------------------|
| 0.85 | 201.73±0.94     |
| 0.90 | 201.73±1.08     |
| 0.95 | 201.73±1.28     |

Dikkat edin, güven olasılığı ne kadar yüksekse, güven aralığı o kadar geniş olur.

## Hipotez Testi

Beyzbol oyuncuları veri setimizde farklı oyuncu rolleri vardır, bunlar aşağıda özetlenebilir (bu tablonun nasıl hesaplanabileceğini görmek için [eşlik eden not defterine](notebook.ipynb) bakın):

| Rol | Boy | Ağırlık | Sayı |
|------|--------|--------|-------|
| Catcher | 72.723684 | 204.328947 | 76 |
| Designated_Hitter | 74.222222 | 220.888889 | 18 |
| First_Baseman | 74.000000 | 213.109091 | 55 |
| Outfielder | 73.010309 | 199.113402 | 194 |
| Relief_Pitcher | 74.374603 | 203.517460 | 315 |
| Second_Baseman | 71.362069 | 184.344828 | 58 |
| Shortstop | 71.903846 | 182.923077 | 52 |
| Starting_Pitcher | 74.719457 | 205.163636 | 221 |
| Third_Baseman | 73.044444 | 200.955556 | 45 |

İlk kalecilerin ortalama boylarının ikinci kalecilerinkinden daha yüksek olduğunu fark edebiliriz. Bu nedenle, **ilk kalecilerin ikinci kalecilerden daha uzun olduğu** sonucuna varabiliriz.

> Bu ifade **bir hipotez** olarak adlandırılır, çünkü bu durumun gerçekten doğru olup olmadığını bilmiyoruz.

Ancak, bu sonuca varmanın her zaman açık bir yolu yoktur. Yukarıdaki tartışmadan, her ortalamanın bir güven aralığına sahip olduğunu ve bu farkın sadece istatistiksel bir hata olabileceğini biliyoruz. Hipotezimizi test etmek için daha resmi bir yönteme ihtiyacımız var.

İlk ve ikinci kalecilerin boyları için güven aralıklarını ayrı ayrı hesaplayalım:

| Güven | İlk Kaleciler | İkinci Kaleciler |
|------------|---------------|----------------|
| 0.85 | 73.62..74.38 | 71.04..71.69 |
| 0.90 | 73.56..74.44 | 70.99..71.73 |
| 0.95 | 73.47..74.53 | 70.92..71.81 |

Hiçbir güven seviyesinde aralıkların örtüşmediğini görebiliriz. Bu, ilk kalecilerin ikinci kalecilerden daha uzun olduğu hipotezimizi kanıtlar.

Daha resmi olarak, çözmeye çalıştığımız problem **iki olasılık dağılımının aynı olup olmadığını** veya en azından aynı parametrelere sahip olup olmadığını görmektir. Dağılıma bağlı olarak, bunun için farklı testler kullanmamız gerekir. Dağılımlarımızın normal olduğunu biliyorsak, **[Student t-testi](https://en.wikipedia.org/wiki/Student%27s_t-test)** uygulayabiliriz.

Student t-testinde, varyansı dikkate alarak ortalamalar arasındaki farkı gösteren **t-değeri** hesaplanır. T-değerinin **student dağılımını** takip ettiği gösterilmiştir, bu da bize belirli bir güven seviyesi **p** için eşik değerini verir (bu hesaplanabilir veya sayısal tablolardan bakılabilir). Daha sonra hipotezi onaylamak veya reddetmek için t-değerini bu eşik değerle karşılaştırırız.

Python'da, birçok faydalı istatistiksel fonksiyon içeren **SciPy** paketini kullanabiliriz. Bu paket, `ttest_ind` fonksiyonunu içerir ve bizim için t-değerini hesaplar, ayrıca güven p-değerinin tersine bakışını yapar, böylece sadece güven seviyesine bakarak sonuca varabiliriz.

Örneğin, ilk ve ikinci kalecilerin boyları arasındaki karşılaştırmamız bize şu sonuçları verir: 
```python
from scipy.stats import ttest_ind

tval, pval = ttest_ind(df.loc[df['Role']=='First_Baseman',['Height']], df.loc[df['Role']=='Designated_Hitter',['Height']],equal_var=False)
print(f"T-value = {tval[0]:.2f}\nP-value: {pval[0]}")
```
```
T-value = 7.65
P-value: 9.137321189738925e-12
```
Bizim durumumuzda, p-değeri oldukça düşük, bu da ilk kalecilerin daha uzun olduğuna dair güçlü bir kanıt olduğunu gösterir.

Test etmek isteyebileceğimiz diğer hipotez türleri de vardır, örneğin:
* Belirli bir örneğin bir dağılıma uyduğunu kanıtlamak. Bizim durumumuzda boyların normal dağıldığını varsaydık, ancak bu resmi istatistiksel doğrulama gerektirir.
* Bir örnek ortalamasının önceden tanımlanmış bir değere karşılık geldiğini kanıtlamak
* Birden fazla örneğin ortalamalarını karşılaştırmak (örneğin, farklı yaş grupları arasındaki mutluluk seviyelerindeki fark)

## Büyük Sayılar Yasası ve Merkezi Limit Teoremi

Normal dağılımın neden bu kadar önemli olduğunun nedenlerinden biri **merkezi limit teoremi**dir. Varsayalım ki, ortalama μ ve varyans σ<sup>2</sup> olan herhangi bir dağılımdan bağımsız N değerleri X<sub>1</sub>, ..., X<sub>N</sub> içeren büyük bir örneğimiz var. O zaman, yeterince büyük N için (diğer bir deyişle, N→∞ olduğunda), Σ<sub>i</sub>X<sub>i</sub> ortalaması normal dağılıma sahip olur, ortalama μ ve varyans σ<sup>2</sup>/N ile.

> Merkezi limit teoremini yorumlamanın başka bir yolu, dağılım ne olursa olsun, herhangi bir rastgele değişken değerlerinin toplamının ortalamasını hesapladığınızda normal dağılıma ulaşırsınız.

Merkezi limit teoreminden ayrıca şu sonuç çıkar: N→∞ olduğunda, örnek ortalamasının μ'ya eşit olma olasılığı 1 olur. Bu, **büyük sayılar yasası** olarak bilinir.

## Kovaryans ve Korelasyon

Veriler arasındaki ilişkileri bulmak, Veri Bilimi'nin yaptığı şeylerden biridir. İki dizinin aynı anda benzer davranış sergilediğinde **korelasyon** gösterdiğini söyleriz, yani ya birlikte yükselir/düşerler ya da bir dizi yükselirken diğeri düşer ve tam tersi. Diğer bir deyişle, iki dizi arasında bir ilişki var gibi görünür.

> Korelasyon, iki dizi arasında nedensel bir ilişki olduğunu mutlaka göstermez; bazen her iki değişken de bazı dış nedenlere bağlı olabilir veya iki dizinin korelasyonu tamamen tesadüfi olabilir. Ancak, güçlü matematiksel korelasyon, iki değişkenin bir şekilde bağlantılı olduğuna dair iyi bir göstergedir.

Matematiksel olarak, iki rastgele değişken arasındaki ilişkiyi gösteren ana kavram **kovaryans**dır ve şu şekilde hesaplanır: Cov(X,Y) = **E**\[(X-**E**(X))(Y-**E**(Y))\]. Her iki değişkenin ortalama değerlerinden sapmalarını hesaplar ve bu sapmaların çarpımını alırız. Eğer her iki değişken birlikte saparsa, çarpım her zaman pozitif bir değer olur ve bu pozitif kovaryansa eklenir. Eğer her iki değişken senkronize olmayan bir şekilde saparsa (yani biri ortalamanın altına düşerken diğeri ortalamanın üstüne çıkarsa), her zaman negatif sayılar elde ederiz ve bu negatif kovaryansa eklenir. Eğer sapmalar bağımsızsa, yaklaşık olarak sıfıra eklenirler.

Kovaryansın mutlak değeri, korelasyonun ne kadar büyük olduğunu bize pek söylemez, çünkü gerçek değerlerin büyüklüğüne bağlıdır. Bunu normalleştirmek için kovaryansı her iki değişkenin standart sapmasına bölebiliriz ve **korelasyon** elde ederiz. İyi olan şey, korelasyonun her zaman [-1,1] aralığında olmasıdır; burada 1, değerler arasında güçlü pozitif korelasyonu, -1 güçlü negatif korelasyonu ve 0 hiçbir korelasyon olmadığını (değişkenler bağımsızdır) gösterir.

**Örnek**: Yukarıda bahsedilen veri setinden beyzbol oyuncularının ağırlıkları ve boyları arasındaki korelasyonu hesaplayabiliriz:
```python
print(np.corrcoef(weights,heights))
```
Sonuç olarak, şu şekilde bir **korelasyon matrisi** elde ederiz:
```
array([[1.        , 0.52959196],
       [0.52959196, 1.        ]])
```

> Korelasyon matrisi C, S<sub>1</sub>, ..., S<sub>n</sub> herhangi bir sayıda giriş dizisi için hesaplanabilir. C<sub>ij</sub> değeri, S<sub>i</sub> ve S<sub>j</sub> arasındaki korelasyonu gösterir ve diyagonal elemanlar her zaman 1'dir (bu aynı zamanda S<sub>i</sub>'nin kendi kendine korelasyonudur).

Bizim durumumuzda, 0.53 değeri bir kişinin ağırlığı ile boyu arasında bir miktar korelasyon olduğunu gösterir. Ayrıca, ilişkiyi görsel olarak görmek için bir değeri diğerine karşı dağılım grafiği yapabiliriz:

![Ağırlık ve boy arasındaki ilişki](../../../../translated_images/weight-height-relationship.3f06bde4ca2aba9974182c4ef037ed602acd0fbbbbe2ca91cefd838a9e66bcf9.tr.png)

> Korelasyon ve kovaryans ile ilgili daha fazla örnek [eşlik eden not defterinde](notebook.ipynb) bulunabilir.

## Sonuç

Bu bölümde şunları öğrendik:

* verilerin temel istatistiksel özellikleri, örneğin ortalama, varyans, mod ve çeyrekler
* rastgele değişkenlerin farklı dağılımları, normal dağılım dahil
* farklı özellikler arasındaki korelasyonu nasıl bulacağımız
* bazı hipotezleri kanıtlamak için matematik ve istatistiklerin sağlam araçlarını nasıl kullanacağımız
* veri örneği verilen rastgele değişken için güven aralıklarını nasıl hesaplayacağımız

Bu, olasılık ve istatistik içinde var olan konuların kesinlikle kapsamlı bir listesi olmasa da, bu kursa iyi bir başlangıç yapmanız için yeterli olmalıdır.

## 🚀 Zorluk

Not defterindeki örnek kodu kullanarak şu hipotezleri test edin: 
1. İlk kaleciler ikinci kalecilerden daha yaşlıdır
2. İlk kaleciler üçüncü kalecilerden daha uzundur
3. Shortstop'lar ikinci kalecilerden daha uzundur

## [Ders sonrası test](https://ff-quizzes.netlify.app/en/ds/)

## Gözden Geçirme ve Kendi Kendine Çalışma

Olasılık ve istatistik o kadar geniş bir konudur ki kendi kursunu hak eder. Teoriye daha derinlemesine dalmak istiyorsanız, aşağıdaki kitaplardan bazılarını okumaya devam edebilirsiniz:

1. [Carlos Fernandez-Granda](https://cims.nyu.edu/~cfgranda/) New York Üniversitesi'nden harika ders notları [Probability and Statistics for Data Science](https://cims.nyu.edu/~cfgranda/pages/stuff/probability_stats_for_DS.pdf) (çevrimiçi olarak mevcut)
1. [Peter ve Andrew Bruce. Practical Statistics for Data Scientists.](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/) [[R'de örnek kod](https://github.com/andrewgbruce/statistics-for-data-scientists)]. 
1. [James D. Miller. Statistics for Data Science](https://www.packtpub.com/product/statistics-for-data-science/9781788290678) [[R'de örnek kod](https://github.com/PacktPublishing/Statistics-for-Data-Science)]

## Ödev

[Küçük Diyabet Çalışması](assignment.md)

## Katkılar

Bu ders [Dmitry Soshnikov](http://soshnikov.com) tarafından ♥️ ile hazırlanmıştır.

---

**Feragatname**:  
Bu belge, AI çeviri hizmeti [Co-op Translator](https://github.com/Azure/co-op-translator) kullanılarak çevrilmiştir. Doğruluk için çaba göstersek de, otomatik çevirilerin hata veya yanlışlıklar içerebileceğini lütfen unutmayın. Belgenin orijinal dili, yetkili kaynak olarak kabul edilmelidir. Kritik bilgiler için profesyonel insan çevirisi önerilir. Bu çevirinin kullanımından kaynaklanan yanlış anlamalar veya yanlış yorumlamalar için sorumluluk kabul etmiyoruz.