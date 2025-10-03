<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d24976d371de57bb657d3127f4195542",
  "translation_date": "2025-10-03T14:00:04+00:00",
  "source_file": "README.md",
  "language_code": "tr"
}
-->
# Veri Bilimi için Başlangıç - Bir Müfredat

Azure Cloud Advocates ekibi olarak Microsoft'ta, Veri Bilimi hakkında 10 haftalık, 20 derslik bir müfredat sunmaktan mutluluk duyuyoruz. Her ders, öncesi ve sonrası için quizler, dersin tamamlanması için yazılı talimatlar, bir çözüm ve bir ödev içerir. Proje tabanlı öğrenme yaklaşımımız, yeni becerilerin kalıcı olmasını sağlayan kanıtlanmış bir yöntemdir.

**Yazarlarımıza içten teşekkürler:** [Jasmine Greenaway](https://www.twitter.com/paladique), [Dmitry Soshnikov](http://soshnikov.com), [Nitya Narasimhan](https://twitter.com/nitya), [Jalen McGee](https://twitter.com/JalenMcG), [Jen Looper](https://twitter.com/jenlooper), [Maud Levy](https://twitter.com/maudstweets), [Tiffany Souterre](https://twitter.com/TiffanySouterre), [Christopher Harrison](https://www.twitter.com/geektrainer).

**🙏 Özel teşekkürler 🙏 [Microsoft Öğrenci Elçileri](https://studentambassadors.microsoft.com/) yazarlarımıza, inceleyicilerimize ve içerik katkıcılarımıza,** özellikle Aaryan Arora, [Aditya Garg](https://github.com/AdityaGarg00), [Alondra Sanchez](https://www.linkedin.com/in/alondra-sanchez-molina/), [Ankita Singh](https://www.linkedin.com/in/ankitasingh007), [Anupam Mishra](https://www.linkedin.com/in/anupam--mishra/), [Arpita Das](https://www.linkedin.com/in/arpitadas01/), ChhailBihari Dubey, [Dibri Nsofor](https://www.linkedin.com/in/dibrinsofor), [Dishita Bhasin](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [Majd Safi](https://www.linkedin.com/in/majd-s/), [Max Blum](https://www.linkedin.com/in/max-blum-6036a1186/), [Miguel Correa](https://www.linkedin.com/in/miguelmque/), [Mohamma Iftekher (Iftu) Ebne Jalal](https://twitter.com/iftu119), [Nawrin Tabassum](https://www.linkedin.com/in/nawrin-tabassum), [Raymond Wangsa Putra](https://www.linkedin.com/in/raymond-wp/), [Rohit Yadav](https://www.linkedin.com/in/rty2423), Samridhi Sharma, [Sanya Sinha](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200), [Sheena Narula](https://www.linkedin.com/in/sheena-narua-n/), [Tauqeer Ahmad](https://www.linkedin.com/in/tauqeerahmad5201/), Yogendrasingh Pawar, [Vidushi Gupta](https://www.linkedin.com/in/vidushi-gupta07/), [Jasleen Sondhi](https://www.linkedin.com/in/jasleen-sondhi/)

|![@sketchthedocs tarafından Sketchnote https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.tr.png)|
|:---:|
| Veri Bilimi için Başlangıç - _[@nitya](https://twitter.com/nitya) tarafından Sketchnote_ |

### 🌐 Çok Dilli Destek

#### GitHub Action ile Destekleniyor (Otomatik ve Her Zaman Güncel)

[Fransızca](../fr/README.md) | [İspanyolca](../es/README.md) | [Almanca](../de/README.md) | [Rusça](../ru/README.md) | [Arapça](../ar/README.md) | [Farsça](../fa/README.md) | [Urduca](../ur/README.md) | [Çince (Basitleştirilmiş)](../zh/README.md) | [Çince (Geleneksel, Macau)](../mo/README.md) | [Çince (Geleneksel, Hong Kong)](../hk/README.md) | [Çince (Geleneksel, Tayvan)](../tw/README.md) | [Japonca](../ja/README.md) | [Korece](../ko/README.md) | [Hintçe](../hi/README.md) | [Bengalce](../bn/README.md) | [Marathi](../mr/README.md) | [Nepalce](../ne/README.md) | [Pencapça (Gurmukhi)](../pa/README.md) | [Portekizce (Portekiz)](../pt/README.md) | [Portekizce (Brezilya)](../br/README.md) | [İtalyanca](../it/README.md) | [Lehçe](../pl/README.md) | [Türkçe](./README.md) | [Yunanca](../el/README.md) | [Tayca](../th/README.md) | [İsveççe](../sv/README.md) | [Danca](../da/README.md) | [Norveççe](../no/README.md) | [Fince](../fi/README.md) | [Felemenkçe](../nl/README.md) | [İbranice](../he/README.md) | [Vietnamca](../vi/README.md) | [Endonezce](../id/README.md) | [Malayca](../ms/README.md) | [Tagalog (Filipince)](../tl/README.md) | [Swahili](../sw/README.md) | [Macarca](../hu/README.md) | [Çekçe](../cs/README.md) | [Slovakça](../sk/README.md) | [Romence](../ro/README.md) | [Bulgarca](../bg/README.md) | [Sırpça (Kiril)](../sr/README.md) | [Hırvatça](../hr/README.md) | [Slovence](../sl/README.md) | [Ukraynaca](../uk/README.md) | [Burma (Myanmar)](../my/README.md)

**Ek dil çevirileri talep etmek isterseniz, desteklenen diller [burada](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md) listelenmiştir.**

#### Topluluğumuza Katılın 
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://aka.ms/ds4beginners/discord)

AI ile öğrenme serimiz devam ediyor, daha fazla bilgi edinin ve [AI ile Öğrenme Serisi](https://aka.ms/learnwithai/discord) etkinliğine 18 - 30 Eylül 2025 tarihleri arasında katılın. GitHub Copilot'u Veri Bilimi için kullanma ipuçları ve püf noktalarını öğrenin.

![AI ile Öğrenme Serisi](../../translated_images/1.2b28cdc6205e26fef6a21817fe5d83ae8b50fbd0a33e9fed0df05845da5b30b6.tr.jpg)

# Öğrenci misiniz?

Aşağıdaki kaynaklarla başlayabilirsiniz:

- [Öğrenci Merkezi sayfası](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) Bu sayfada başlangıç kaynakları, öğrenci paketleri ve hatta ücretsiz sertifika kuponu alma yollarını bulabilirsiniz. Bu sayfayı sık sık kontrol etmek isteyebilirsiniz çünkü içeriği en az ayda bir değiştiriyoruz.
- [Microsoft Learn Öğrenci Elçileri](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) Küresel bir öğrenci elçileri topluluğuna katılın, bu sizin Microsoft'a giriş yolunuz olabilir.

# Başlarken

## 📚 Belgeler

- **[Kurulum Kılavuzu](INSTALLATION.md)** - Yeni başlayanlar için adım adım kurulum talimatları
- **[Kullanım Kılavuzu](USAGE.md)** - Örnekler ve yaygın iş akışları
- **[Sorun Giderme](TROUBLESHOOTING.md)** - Yaygın sorunlara çözümler
- **[Katkı Kılavuzu](CONTRIBUTING.md)** - Bu projeye nasıl katkıda bulunabilirsiniz
- **[Öğretmenler için](for-teachers.md)** - Öğretim rehberi ve sınıf kaynakları

## 👨‍🎓 Öğrenciler İçin
> **Tamamen Yeni Başlayanlar**: Veri bilimine yeni mi başlıyorsunuz? [Yeni başlayanlar için örnekler](examples/README.md) ile başlayın! Bu basit, iyi açıklanmış örnekler, tam müfredata dalmadan önce temel bilgileri anlamanıza yardımcı olacaktır.
> **[Öğrenciler](https://aka.ms/student-page)**: Bu müfredatı kendi başınıza kullanmak için tüm repo'yu fork edin ve alıştırmaları kendi başınıza tamamlayın, bir ön ders quiz'i ile başlayarak. Ardından dersi okuyun ve diğer aktiviteleri tamamlayın. Dersleri anlayarak projeleri oluşturmaya çalışın, çözüm kodunu kopyalamaktan kaçının; ancak bu kod, her proje odaklı dersin /solutions klasörlerinde mevcuttur. Başka bir fikir, arkadaşlarınızla bir çalışma grubu oluşturup içeriği birlikte incelemek olabilir. Daha fazla çalışma için [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum) öneriyoruz.

**Hızlı Başlangıç:**
1. Ortamınızı kurmak için [Kurulum Kılavuzu](INSTALLATION.md)'nu kontrol edin
2. Müfredatla nasıl çalışacağınızı öğrenmek için [Kullanım Kılavuzu](USAGE.md)'nu inceleyin
3. 1. Dersten başlayarak sırayla ilerleyin
4. Destek için [Discord topluluğumuza](https://aka.ms/ds4beginners/discord) katılın

## 👩‍🏫 Öğretmenler İçin

> **Öğretmenler**: Bu müfredatı nasıl kullanabileceğinizle ilgili [bazı öneriler](for-teachers.md) ekledik. Geri bildirimlerinizi [tartışma forumumuzda](https://github.com/microsoft/Data-Science-For-Beginners/discussions) paylaşabilirsiniz!

## Ekibi Tanıyın

[![Tanıtım videosu](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "Tanıtım videosu")

**Gif** [Mohit Jaisal](https://www.linkedin.com/in/mohitjaisal) tarafından

> 🎥 Yukarıdaki görsele tıklayarak proje ve onu oluşturan kişiler hakkında bir video izleyebilirsiniz!

## Pedagoji

Bu müfredatı oluştururken iki pedagojik ilkeyi benimsedik: proje tabanlı olmasını sağlamak ve sık sık quizler içermesi. Bu serinin sonunda, öğrenciler veri biliminin temel ilkelerini, etik kavramları, veri hazırlama yöntemlerini, veriyle çalışma yollarını, veri görselleştirme, veri analizi, veri biliminin gerçek dünya uygulamaları ve daha fazlasını öğrenmiş olacaklar.
Ayrıca, ders öncesi yapılan düşük riskli bir test, öğrencinin bir konuyu öğrenmeye yönelik niyetini belirlerken, ders sonrası yapılan ikinci bir test, bilgilerin daha iyi pekişmesini sağlar. Bu müfredat esnek ve eğlenceli olacak şekilde tasarlandı ve tamamı veya bir kısmı alınabilir. Projeler küçük başlar ve 10 haftalık döngünün sonunda giderek daha karmaşık hale gelir.

> [Davranış Kuralları](CODE_OF_CONDUCT.md), [Katkıda Bulunma](CONTRIBUTING.md), [Çeviri](TRANSLATIONS.md) yönergelerimizi inceleyin. Yapıcı geri bildirimlerinizi memnuniyetle karşılıyoruz!

## Her ders şunları içerir:

- İsteğe bağlı çizim notları
- İsteğe bağlı ek video
- Ders öncesi ısınma testi
- Yazılı ders
- Proje tabanlı dersler için, projeyi nasıl oluşturacağınızı adım adım anlatan rehberler
- Bilgi kontrolleri
- Bir meydan okuma
- Ek okuma materyalleri
- Ödev
- [Ders sonrası test](https://ff-quizzes.netlify.app/en/)

> **Testler hakkında bir not**: Tüm testler Quiz-App klasöründe yer alır ve her biri üç sorudan oluşan toplam 40 test içerir. Derslerin içinde bağlantılıdır, ancak test uygulaması yerel olarak çalıştırılabilir veya Azure'a dağıtılabilir; `quiz-app` klasöründeki talimatları takip edin. Testler kademeli olarak yerelleştirilmektedir.

## 🎓 Yeni Başlayanlar İçin Örnekler

**Veri Bilimine Yeni mi Başlıyorsunuz?** Başlamanıza yardımcı olmak için basit, iyi açıklanmış kod içeren özel bir [örnekler dizini](examples/README.md) oluşturduk:

- 🌟 **Merhaba Dünya** - İlk veri bilimi programınız
- 📂 **Veri Yükleme** - Veri setlerini okumayı ve keşfetmeyi öğrenin
- 📊 **Basit Analiz** - İstatistik hesaplayın ve desenleri bulun
- 📈 **Temel Görselleştirme** - Grafikler ve tablolar oluşturun
- 🔬 **Gerçek Dünya Projesi** - Baştan sona tam bir iş akışı

Her örnek, her adımı açıklayan ayrıntılı yorumlar içerir, bu da onu tamamen yeni başlayanlar için mükemmel hale getirir!

👉 **[Örneklerle başlayın](examples/README.md)** 👈

## Dersler

|![ @sketchthedocs tarafından çizim notu https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.tr.png)|
|:---:|
| Veri Bilimi Yeni Başlayanlar İçin: Yol Haritası - _[@nitya](https://twitter.com/nitya) tarafından çizim notu_ |

| Ders Numarası | Konu | Ders Grubu | Öğrenme Hedefleri | Bağlantılı Ders | Yazar |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | Veri Bilimini Tanımlama | [Giriş](1-Introduction/README.md) | Veri biliminin temel kavramlarını ve yapay zeka, makine öğrenimi ve büyük veri ile ilişkisini öğrenin. | [ders](1-Introduction/01-defining-data-science/README.md) [video](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | Veri Bilimi Etiği | [Giriş](1-Introduction/README.md) | Veri etiği kavramları, zorlukları ve çerçeveleri. | [ders](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | Veriyi Tanımlama | [Giriş](1-Introduction/README.md) | Verinin nasıl sınıflandırıldığı ve yaygın kaynakları. | [ders](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | İstatistik ve Olasılığa Giriş | [Giriş](1-Introduction/README.md) | Veriyi anlamak için olasılık ve istatistik matematiksel teknikleri. | [ders](1-Introduction/04-stats-and-probability/README.md) [video](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | İlişkisel Veri ile Çalışma | [Veri ile Çalışma](2-Working-With-Data/README.md) | İlişkisel veriye giriş ve Structured Query Language (SQL) olarak bilinen dili kullanarak ilişkisel veriyi keşfetme ve analiz etmenin temelleri. | [ders](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | NoSQL Veri ile Çalışma | [Veri ile Çalışma](2-Working-With-Data/README.md) | İlişkisel olmayan veriye giriş, çeşitli türleri ve belge veritabanlarını keşfetme ve analiz etmenin temelleri. | [ders](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | Python ile Çalışma | [Veri ile Çalışma](2-Working-With-Data/README.md) | Pandas gibi kütüphanelerle veri keşfi için Python kullanmanın temelleri. Python programlama hakkında temel bir anlayış önerilir. | [ders](2-Working-With-Data/07-python/README.md) [video](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | Veri Hazırlama | [Veri ile Çalışma](2-Working-With-Data/README.md) | Eksik, hatalı veya eksik verilerle başa çıkmak için veri temizleme ve dönüştürme teknikleri üzerine konular. | [ders](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | Miktarları Görselleştirme | [Veri Görselleştirme](3-Data-Visualization/README.md) | Matplotlib kullanarak kuş verilerini görselleştirmeyi öğrenin 🦆 | [ders](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | Veri Dağılımlarını Görselleştirme | [Veri Görselleştirme](3-Data-Visualization/README.md) | Bir aralık içindeki gözlemleri ve eğilimleri görselleştirme. | [ders](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | Oranları Görselleştirme | [Veri Görselleştirme](3-Data-Visualization/README.md) | Ayrık ve gruplandırılmış yüzdeleri görselleştirme. | [ders](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | İlişkileri Görselleştirme | [Veri Görselleştirme](3-Data-Visualization/README.md) | Veri setleri ve değişkenleri arasındaki bağlantıları ve korelasyonları görselleştirme. | [ders](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | Anlamlı Görselleştirmeler | [Veri Görselleştirme](3-Data-Visualization/README.md) | Sorun çözme ve içgörüler için görselleştirmelerinizi değerli hale getirmek için teknikler ve rehberlik. | [ders](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | Veri Bilimi Yaşam Döngüsüne Giriş | [Yaşam Döngüsü](4-Data-Science-Lifecycle/README.md) | Veri bilimi yaşam döngüsüne giriş ve veri edinme ve çıkarma adımı. | [ders](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | Analiz | [Yaşam Döngüsü](4-Data-Science-Lifecycle/README.md) | Veri bilimi yaşam döngüsünün bu aşaması, veriyi analiz etme tekniklerine odaklanır. | [ders](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | İletişim | [Yaşam Döngüsü](4-Data-Science-Lifecycle/README.md) | Veri bilimi yaşam döngüsünün bu aşaması, veriden elde edilen içgörüleri karar vericilerin anlamasını kolaylaştıracak şekilde sunmaya odaklanır. | [ders](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | Bulutta Veri Bilimi | [Bulut Verisi](5-Data-Science-In-Cloud/README.md) | Bulutta veri bilimine ve avantajlarına giriş. | [ders](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) ve [Maud](https://twitter.com/maudstweets) |
| 18 | Bulutta Veri Bilimi | [Bulut Verisi](5-Data-Science-In-Cloud/README.md) | Düşük Kod araçları kullanarak modelleri eğitme. |[ders](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) ve [Maud](https://twitter.com/maudstweets) |
| 19 | Bulutta Veri Bilimi | [Bulut Verisi](5-Data-Science-In-Cloud/README.md) | Azure Machine Learning Studio ile modelleri dağıtma. | [ders](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) ve [Maud](https://twitter.com/maudstweets) |
| 20 | Vahşi Doğada Veri Bilimi | [Vahşi Doğada](6-Data-Science-In-Wild/README.md) | Gerçek dünyada veri bilimi odaklı projeler. | [ders](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

Bu örneği bir Codespace'de açmak için şu adımları izleyin:
1. Kod açılır menüsüne tıklayın ve Codespaces ile Aç seçeneğini seçin.
2. Panonun altındaki + Yeni codespace seçeneğini seçin.
Daha fazla bilgi için [GitHub belgelerine](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace) göz atın.

## VSCode Remote - Containers
Yerel makinenizi ve VSCode'u kullanarak bu depoyu bir konteynerde açmak için VS Code Remote - Containers uzantısını kullanarak şu adımları izleyin:

1. İlk kez bir geliştirme konteyneri kullanıyorsanız, sisteminizin ön gereksinimleri karşıladığından emin olun (örneğin, Docker yüklü olmalı) [başlangıç belgelerinde](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started).

Bu depoyu kullanmak için, ya depoyu izole bir Docker hacminde açabilirsiniz:

**Not**: Arka planda, bu işlem, kaynak kodu yerel dosya sistemi yerine bir Docker hacminde klonlamak için Remote-Containers: **Clone Repository in Container Volume...** komutunu kullanacaktır. [Hacimler](https://docs.docker.com/storage/volumes/) konteyner verilerini kalıcı hale getirmek için tercih edilen mekanizmadır.

Ya da yerel olarak klonlanmış veya indirilmiş bir depo sürümünü açabilirsiniz:

- Bu depoyu yerel dosya sisteminize klonlayın.
- F1 tuşuna basın ve **Remote-Containers: Open Folder in Container...** komutunu seçin.
- Bu klasörün klonlanmış kopyasını seçin, konteynerin başlamasını bekleyin ve şeyleri deneyin.

## Çevrimdışı erişim

Bu belgeleri [Docsify](https://docsify.js.org/#/) kullanarak çevrimdışı çalıştırabilirsiniz. Bu depoyu çatallayın, [Docsify'i yükleyin](https://docsify.js.org/#/quickstart) yerel makinenize, ardından bu deponun kök klasöründe `docsify serve` yazın. Web sitesi localhost'ta 3000 portunda çalıştırılacaktır: `localhost:3000`.

> Not, defterler Docsify üzerinden görüntülenmeyecektir, bu yüzden bir defteri çalıştırmanız gerektiğinde, bunu ayrı olarak Python çekirdeği çalıştıran VS Code'da yapın.

## Diğer Müfredatlar

Ekibimiz başka müfredatlar da üretiyor! Şunlara göz atın:

- [Yeni Başlayanlar İçin Edge AI](https://aka.ms/edgeai-for-beginners)
- [Yeni Başlayanlar İçin AI Ajanları](https://aka.ms/ai-agents-beginners)
- [Yeni Başlayanlar İçin Üretken AI](https://aka.ms/genai-beginners)
- [Yeni Başlayanlar İçin Üretken AI .NET](https://github.com/microsoft/Generative-AI-for-beginners-dotnet)
- [JavaScript ile Üretken AI](https://github.com/microsoft/generative-ai-with-javascript)
- [Java ile Üretken AI](https://aka.ms/genaijava)
- [Yeni Başlayanlar İçin AI](https://aka.ms/ai-beginners)
- [Yeni Başlayanlar İçin Veri Bilimi](https://aka.ms/datascience-beginners)
- [Yeni Başlayanlar İçin Bash](https://github.com/microsoft/bash-for-beginners)
- [Yeni Başlayanlar İçin ML](https://aka.ms/ml-beginners)
- [Yeni Başlayanlar İçin Siber Güvenlik](https://github.com/microsoft/Security-101) 
- [Yeni Başlayanlar İçin Web Geliştirme](https://aka.ms/webdev-beginners)
- [Yeni Başlayanlar İçin IoT](https://aka.ms/iot-beginners)
- [Yeni Başlayanlar İçin Makine Öğrenimi](https://aka.ms/ml-beginners)
- [Yeni Başlayanlar İçin XR Geliştirme](https://aka.ms/xr-dev-for-beginners)
- [GitHub Copilot ile Yapay Zeka Eşli Programlamayı Öğrenme](https://aka.ms/GitHubCopilotAI)
- [Yeni Başlayanlar için XR Geliştirme](https://github.com/microsoft/xr-development-for-beginners)
- [C#/.NET Geliştiricileri için GitHub Copilot'u Öğrenme](https://github.com/microsoft/mastering-github-copilot-for-dotnet-csharp-developers)
- [Kendi Copilot Maceranı Seç](https://github.com/microsoft/CopilotAdventures)

## Yardım Alma

**Sorunlarla mı karşılaşıyorsunuz?** Yaygın problemler için çözümler bulmak adına [Sorun Giderme Kılavuzumuza](TROUBLESHOOTING.md) göz atın.

Eğer takılırsanız veya yapay zeka uygulamaları oluşturma konusunda sorularınız olursa, şu topluluğa katılın:

[![Azure AI Foundry Discord](https://img.shields.io/badge/Discord-Azure_AI_Foundry_Community_Discord-blue?style=for-the-badge&logo=discord&color=5865f2&logoColor=fff)](https://aka.ms/foundry/discord)

Ürünle ilgili geri bildirimde bulunmak veya geliştirme sırasında hatalarla karşılaşmak için şu adresi ziyaret edin:

[![Azure AI Foundry Developer Forum](https://img.shields.io/badge/GitHub-Azure_AI_Foundry_Developer_Forum-blue?style=for-the-badge&logo=github&color=000000&logoColor=fff)](https://aka.ms/foundry/forum)

---

**Feragatname**:  
Bu belge, AI çeviri hizmeti [Co-op Translator](https://github.com/Azure/co-op-translator) kullanılarak çevrilmiştir. Doğruluk için çaba göstersek de, otomatik çevirilerin hata veya yanlışlıklar içerebileceğini lütfen unutmayın. Belgenin orijinal dili, yetkili kaynak olarak kabul edilmelidir. Kritik bilgiler için profesyonel insan çevirisi önerilir. Bu çevirinin kullanımından kaynaklanan yanlış anlamalar veya yanlış yorumlamalar için sorumluluk kabul etmiyoruz.