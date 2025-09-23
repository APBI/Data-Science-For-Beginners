<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "ae529efe508173a92d4019d86744ec00",
  "translation_date": "2025-09-23T08:56:38+00:00",
  "source_file": "README.md",
  "language_code": "hi"
}
-->
# डेटा साइंस के शुरुआती लोगों के लिए - एक पाठ्यक्रम

Azure Cloud Advocates, Microsoft द्वारा प्रस्तुत, 10 सप्ताह का, 20 पाठों का पाठ्यक्रम, जो पूरी तरह से डेटा साइंस पर आधारित है। हर पाठ में प्री-लेसन और पोस्ट-लेसन क्विज़, लिखित निर्देश, समाधान और असाइनमेंट शामिल हैं। हमारा प्रोजेक्ट-आधारित शिक्षण तरीका आपको सीखने के साथ-साथ निर्माण करने का मौका देता है, जो नई स्किल्स को लंबे समय तक याद रखने का एक सिद्ध तरीका है।

**हमारे लेखकों को हार्दिक धन्यवाद:** [जैस्मिन ग्रीनवे](https://www.twitter.com/paladique), [दिमित्री सॉश्निकोव](http://soshnikov.com), [नित्या नरसिम्हन](https://twitter.com/nitya), [जालेन मैक्गी](https://twitter.com/JalenMcG), [जेन लूपर](https://twitter.com/jenlooper), [मॉड लेवी](https://twitter.com/maudstweets), [टिफ़नी सॉटर](https://twitter.com/TiffanySouterre), [क्रिस्टोफर हैरिसन](https://www.twitter.com/geektrainer)।

**🙏 विशेष धन्यवाद 🙏 हमारे [Microsoft Student Ambassador](https://studentambassadors.microsoft.com/) लेखकों, समीक्षकों और सामग्री योगदानकर्ताओं को,** विशेष रूप से आर्यन अरोड़ा, [आदित्य गर्ग](https://github.com/AdityaGarg00), [अलोंड्रा सांचेज़](https://www.linkedin.com/in/alondra-sanchez-molina/), [अंकिता सिंह](https://www.linkedin.com/in/ankitasingh007), [अनुपम मिश्रा](https://www.linkedin.com/in/anupam--mishra/), [अर्पिता दास](https://www.linkedin.com/in/arpitadas01/), छैल बिहारी दुबे, [डिब्री नसोफर](https://www.linkedin.com/in/dibrinsofor), [दिशिता भसीन](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [मज्द साफी](https://www.linkedin.com/in/majd-s/), [मैक्स ब्लम](https://www.linkedin.com/in/max-blum-6036a1186/), [मिगुएल कोरेया](https://www.linkedin.com/in/miguelmque/), [मोहम्मा इफ्तेखर (इफ्तु) इब्ने जलाल](https://twitter.com/iftu119), [नवरिन तबस्सुम](https://www.linkedin.com/in/nawrin-tabassum), [रेमंड वांगसा पुत्रा](https://www.linkedin.com/in/raymond-wp/), [रोहित यादव](https://www.linkedin.com/in/rty2423), समृद्धि शर्मा, [सान्या सिन्हा](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200), [शीना नरूला](https://www.linkedin.com/in/sheena-narua-n/), [तौकीर अहमद](https://www.linkedin.com/in/tauqeerahmad5201/), योगेंद्रसिंह पवार, [विदुषी गुप्ता](https://www.linkedin.com/in/vidushi-gupta07/), [जसलीन सोनधी](https://www.linkedin.com/in/jasleen-sondhi/)।

|![स्केच नोट @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.hi.png)|
|:---:|
| शुरुआती लोगों के लिए डेटा साइंस - _स्केच नोट [@nitya](https://twitter.com/nitya)_ द्वारा |

### 🌐 बहुभाषी समर्थन

#### GitHub Action के माध्यम से समर्थित (स्वचालित और हमेशा अद्यतन)

[French](../fr/README.md) | [Spanish](../es/README.md) | [German](../de/README.md) | [Russian](../ru/README.md) | [Arabic](../ar/README.md) | [Persian (Farsi)](../fa/README.md) | [Urdu](../ur/README.md) | [Chinese (Simplified)](../zh/README.md) | [Chinese (Traditional, Macau)](../mo/README.md) | [Chinese (Traditional, Hong Kong)](../hk/README.md) | [Chinese (Traditional, Taiwan)](../tw/README.md) | [Japanese](../ja/README.md) | [Korean](../ko/README.md) | [Hindi](./README.md) | [Bengali](../bn/README.md) | [Marathi](../mr/README.md) | [Nepali](../ne/README.md) | [Punjabi (Gurmukhi)](../pa/README.md) | [Portuguese (Portugal)](../pt/README.md) | [Portuguese (Brazil)](../br/README.md) | [Italian](../it/README.md) | [Polish](../pl/README.md) | [Turkish](../tr/README.md) | [Greek](../el/README.md) | [Thai](../th/README.md) | [Swedish](../sv/README.md) | [Danish](../da/README.md) | [Norwegian](../no/README.md) | [Finnish](../fi/README.md) | [Dutch](../nl/README.md) | [Hebrew](../he/README.md) | [Vietnamese](../vi/README.md) | [Indonesian](../id/README.md) | [Malay](../ms/README.md) | [Tagalog (Filipino)](../tl/README.md) | [Swahili](../sw/README.md) | [Hungarian](../hu/README.md) | [Czech](../cs/README.md) | [Slovak](../sk/README.md) | [Romanian](../ro/README.md) | [Bulgarian](../bg/README.md) | [Serbian (Cyrillic)](../sr/README.md) | [Croatian](../hr/README.md) | [Slovenian](../sl/README.md) | [Ukrainian](../uk/README.md) | [Burmese (Myanmar)](../my/README.md)

**यदि आप अतिरिक्त भाषाओं में अनुवाद चाहते हैं, तो समर्थित भाषाओं की सूची [यहां](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md) दी गई है।**

#### हमारे समुदाय से जुड़ें 
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://aka.ms/ds4beginners/discord)

हमारे पास AI के साथ सीखने की एक श्रृंखला चल रही है। अधिक जानें और [Learn with AI Series](https://aka.ms/learnwithai/discord) में 18 - 30 सितंबर, 2025 तक शामिल हों। आपको GitHub Copilot का उपयोग करने के टिप्स और ट्रिक्स मिलेंगे।

![AI के साथ सीखने की श्रृंखला](../../translated_images/1.2b28cdc6205e26fef6a21817fe5d83ae8b50fbd0a33e9fed0df05845da5b30b6.hi.jpg)

# क्या आप एक छात्र हैं?

इन संसाधनों से शुरुआत करें:

- [स्टूडेंट हब पेज](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum): इस पेज पर आपको शुरुआती संसाधन, स्टूडेंट पैक्स और यहां तक कि मुफ्त प्रमाणपत्र वाउचर पाने के तरीके मिलेंगे। यह एक ऐसा पेज है जिसे आप बुकमार्क करना चाहेंगे और समय-समय पर चेक करना चाहेंगे क्योंकि हम कम से कम मासिक रूप से सामग्री बदलते हैं।
- [Microsoft Learn Student Ambassadors](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum): छात्र एंबेसडर के वैश्विक समुदाय में शामिल हों, यह Microsoft में आपका प्रवेश द्वार हो सकता है।

# शुरुआत करें

> **शिक्षक**: हमने [कुछ सुझाव शामिल किए हैं](for-teachers.md) कि इस पाठ्यक्रम का उपयोग कैसे करें। हमें आपके फीडबैक की आवश्यकता है [हमारे चर्चा मंच में](https://github.com/microsoft/Data-Science-For-Beginners/discussions)!

> **[छात्र](https://aka.ms/student-page)**: इस पाठ्यक्रम का उपयोग अपने आप करने के लिए, पूरे रिपॉजिटरी को फोर्क करें और अपने आप अभ्यास करें, प्री-लेक्चर क्विज़ से शुरुआत करें। फिर लेक्चर पढ़ें और बाकी गतिविधियों को पूरा करें। कोशिश करें कि प्रोजेक्ट्स को समझकर बनाएं, न कि समाधान कोड को कॉपी करके; हालांकि, वह कोड प्रत्येक प्रोजेक्ट-आधारित पाठ में /solutions फोल्डर में उपलब्ध है। एक और विचार यह हो सकता है कि दोस्तों के साथ एक अध्ययन समूह बनाएं और सामग्री को एक साथ पढ़ें। आगे की पढ़ाई के लिए, हम [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum) की सिफारिश करते हैं।

## टीम से मिलें

[![प्रोमो वीडियो](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "प्रोमो वीडियो")

**Gif द्वारा** [मोहित जैसल](https://www.linkedin.com/in/mohitjaisal)

> 🎥 ऊपर दी गई छवि पर क्लिक करें इस प्रोजेक्ट और इसे बनाने वाले लोगों के बारे में वीडियो देखने के लिए!

## शिक्षण पद्धति

हमने इस पाठ्यक्रम को बनाते समय दो शिक्षण सिद्धांतों को चुना है: यह सुनिश्चित करना कि यह प्रोजेक्ट-आधारित है और इसमें बार-बार क्विज़ शामिल हैं। इस श्रृंखला के अंत तक, छात्र डेटा साइंस के बुनियादी सिद्धांतों को सीखेंगे, जिनमें नैतिक अवधारणाएं, डेटा तैयारी, डेटा के साथ काम करने के विभिन्न तरीके, डेटा विज़ुअलाइज़ेशन, डेटा विश्लेषण, डेटा साइंस के वास्तविक जीवन के उपयोग के मामले और अधिक शामिल हैं।

इसके अलावा, कक्षा से पहले एक कम दबाव वाला क्विज़ छात्र को विषय सीखने के लिए प्रेरित करता है, जबकि कक्षा के बाद दूसरा क्विज़ आगे की जानकारी को बनाए रखने में मदद करता है। यह पाठ्यक्रम लचीला और मजेदार बनाया गया है और इसे पूरे या आंशिक रूप से लिया जा सकता है। प्रोजेक्ट्स छोटे से शुरू होते हैं और 10 सप्ताह के चक्र के अंत तक धीरे-धीरे जटिल हो जाते हैं।

> हमारा [आचार संहिता](CODE_OF_CONDUCT.md), [योगदान](CONTRIBUTING.md), [अनुवाद](TRANSLATIONS.md) दिशानिर्देश देखें। हम आपके रचनात्मक फीडबैक का स्वागत करते हैं!

## प्रत्येक पाठ में शामिल हैं:

- वैकल्पिक स्केच नोट
- वैकल्पिक पूरक वीडियो
- प्री-लेसन वार्मअप क्विज़
- लिखित पाठ
- प्रोजेक्ट-आधारित पाठों के लिए, प्रोजेक्ट बनाने के लिए चरण-दर-चरण गाइड
- ज्ञान जांच
- एक चुनौती
- पूरक पढ़ाई
- असाइनमेंट
- [पोस्ट-लेसन क्विज़](https://ff-quizzes.netlify.app/en/)

> **क्विज़ के बारे में एक नोट**: सभी क्विज़ Quiz-App फोल्डर में शामिल हैं, कुल 40 क्विज़, प्रत्येक में तीन प्रश्न। वे पाठों के भीतर से लिंक किए गए हैं, लेकिन क्विज़ ऐप को स्थानीय रूप से चलाया जा सकता है या Azure पर तैनात किया जा सकता है; `quiz-app` फोल्डर में दिए गए निर्देशों का पालन करें। उन्हें धीरे-धीरे स्थानीयकृत किया जा रहा है।

## पाठ


|![ Sketchnote by @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.hi.png)|
|:---:|
| डेटा साइंस फॉर बिगिनर्स: रोडमैप - _स्केच नोट [@nitya](https://twitter.com/nitya) द्वारा_ |

| पाठ संख्या | विषय | पाठ समूह | सीखने के उद्देश्य | लिंक किया गया पाठ | लेखक |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | डेटा साइंस की परिभाषा | [परिचय](1-Introduction/README.md) | डेटा साइंस के पीछे के मूलभूत सिद्धांतों को समझें और यह कृत्रिम बुद्धिमत्ता, मशीन लर्निंग और बिग डेटा से कैसे संबंधित है। | [पाठ](1-Introduction/01-defining-data-science/README.md) [वीडियो](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | डेटा साइंस नैतिकता | [परिचय](1-Introduction/README.md) | डेटा नैतिकता के सिद्धांत, चुनौतियाँ और ढांचे। | [पाठ](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | डेटा की परिभाषा | [परिचय](1-Introduction/README.md) | डेटा को कैसे वर्गीकृत किया जाता है और इसके सामान्य स्रोत। | [पाठ](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | सांख्यिकी और संभावना का परिचय | [परिचय](1-Introduction/README.md) | डेटा को समझने के लिए संभावना और सांख्यिकी की गणितीय तकनीकें। | [पाठ](1-Introduction/04-stats-and-probability/README.md) [वीडियो](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | रिलेशनल डेटा के साथ काम करना | [डेटा के साथ काम करना](2-Working-With-Data/README.md) | रिलेशनल डेटा का परिचय और SQL (जिसे "सी-क्वेल" कहा जाता है) के साथ रिलेशनल डेटा का अन्वेषण और विश्लेषण करने की मूल बातें। | [पाठ](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | NoSQL डेटा के साथ काम करना | [डेटा के साथ काम करना](2-Working-With-Data/README.md) | गैर-रिलेशनल डेटा का परिचय, इसके विभिन्न प्रकार और डॉक्यूमेंट डेटाबेस का अन्वेषण और विश्लेषण करने की मूल बातें। | [पाठ](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | Python के साथ काम करना | [डेटा के साथ काम करना](2-Working-With-Data/README.md) | Pandas जैसी लाइब्रेरी के साथ डेटा अन्वेषण के लिए Python का उपयोग करने की मूल बातें। Python प्रोग्रामिंग की बुनियादी समझ की सिफारिश की जाती है। | [पाठ](2-Working-With-Data/07-python/README.md) [वीडियो](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | डेटा तैयारी | [डेटा के साथ काम करना](2-Working-With-Data/README.md) | डेटा को साफ करने और बदलने के लिए तकनीकों पर चर्चा, ताकि गायब, गलत या अधूरी जानकारी की चुनौतियों को संभाला जा सके। | [पाठ](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | मात्राओं का विज़ुअलाइज़ेशन | [डेटा विज़ुअलाइज़ेशन](3-Data-Visualization/README.md) | Matplotlib का उपयोग करके पक्षी डेटा 🦆 को विज़ुअलाइज़ करना सीखें। | [पाठ](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | डेटा वितरण का विज़ुअलाइज़ेशन | [डेटा विज़ुअलाइज़ेशन](3-Data-Visualization/README.md) | अंतराल के भीतर अवलोकन और रुझानों को विज़ुअलाइज़ करना। | [पाठ](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | अनुपात का विज़ुअलाइज़ेशन | [डेटा विज़ुअलाइज़ेशन](3-Data-Visualization/README.md) | अलग-अलग और समूहित प्रतिशत को विज़ुअलाइज़ करना। | [पाठ](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | संबंधों का विज़ुअलाइज़ेशन | [डेटा विज़ुअलाइज़ेशन](3-Data-Visualization/README.md) | डेटा सेट और उनके वेरिएबल्स के बीच कनेक्शन और सहसंबंध को विज़ुअलाइज़ करना। | [पाठ](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | सार्थक विज़ुअलाइज़ेशन | [डेटा विज़ुअलाइज़ेशन](3-Data-Visualization/README.md) | प्रभावी समस्या समाधान और अंतर्दृष्टि के लिए अपने विज़ुअलाइज़ेशन को मूल्यवान बनाने के लिए तकनीक और मार्गदर्शन। | [पाठ](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | डेटा साइंस जीवनचक्र का परिचय | [जीवनचक्र](4-Data-Science-Lifecycle/README.md) | डेटा साइंस जीवनचक्र का परिचय और डेटा को प्राप्त करने और निकालने का पहला चरण। | [पाठ](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | विश्लेषण | [जीवनचक्र](4-Data-Science-Lifecycle/README.md) | डेटा साइंस जीवनचक्र का यह चरण डेटा का विश्लेषण करने की तकनीकों पर केंद्रित है। | [पाठ](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | संचार | [जीवनचक्र](4-Data-Science-Lifecycle/README.md) | डेटा से अंतर्दृष्टि को इस तरह प्रस्तुत करना कि निर्णय लेने वालों के लिए इसे समझना आसान हो। | [पाठ](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | क्लाउड में डेटा साइंस | [क्लाउड डेटा](5-Data-Science-In-Cloud/README.md) | क्लाउड में डेटा साइंस और इसके लाभों का परिचय। | [पाठ](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) और [Maud](https://twitter.com/maudstweets) |
| 18 | क्लाउड में डेटा साइंस | [क्लाउड डेटा](5-Data-Science-In-Cloud/README.md) | लो कोड टूल्स का उपयोग करके मॉडल को प्रशिक्षित करना। |[पाठ](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) और [Maud](https://twitter.com/maudstweets) |
| 19 | क्लाउड में डेटा साइंस | [क्लाउड डेटा](5-Data-Science-In-Cloud/README.md) | Azure Machine Learning Studio के साथ मॉडल को तैनात करना। | [पाठ](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) और [Maud](https://twitter.com/maudstweets) |
| 20 | वास्तविक दुनिया में डेटा साइंस | [वास्तविक दुनिया में](6-Data-Science-In-Wild/README.md) | वास्तविक दुनिया में डेटा साइंस संचालित परियोजनाएँ। | [पाठ](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

Codespace में इस सैंपल को खोलने के लिए इन चरणों का पालन करें:
1. Code ड्रॉप-डाउन मेनू पर क्लिक करें और Open with Codespaces विकल्प चुनें।
2. पैन के नीचे + New codespace चुनें।
अधिक जानकारी के लिए, [GitHub दस्तावेज़](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace) देखें।

## VSCode Remote - Containers
अपने स्थानीय मशीन और VSCode का उपयोग करके इस रिपॉजिटरी को कंटेनर में खोलने के लिए इन चरणों का पालन करें:

1. यदि यह पहली बार है जब आप डेवलपमेंट कंटेनर का उपयोग कर रहे हैं, तो कृपया सुनिश्चित करें कि आपका सिस्टम प्री-रिक्वायरमेंट्स को पूरा करता है (जैसे कि Docker इंस्टॉल हो) [शुरुआती दस्तावेज़](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started) में।

इस रिपॉजिटरी का उपयोग करने के लिए, आप या तो इसे एक अलग Docker वॉल्यूम में खोल सकते हैं:

**नोट**: अंदर ही अंदर, यह Remote-Containers: **Clone Repository in Container Volume...** कमांड का उपयोग करेगा ताकि स्रोत कोड को स्थानीय फाइल सिस्टम के बजाय Docker वॉल्यूम में क्लोन किया जा सके। [Volumes](https://docs.docker.com/storage/volumes/) कंटेनर डेटा को बनाए रखने के लिए पसंदीदा तंत्र हैं।

या स्थानीय रूप से क्लोन की गई या डाउनलोड की गई रिपॉजिटरी खोलें:

- इस रिपॉजिटरी को अपने स्थानीय फाइल सिस्टम पर क्लोन करें।
- F1 दबाएं और **Remote-Containers: Open Folder in Container...** कमांड चुनें।
- इस फ़ोल्डर की क्लोन की गई कॉपी चुनें, कंटेनर के शुरू होने की प्रतीक्षा करें, और चीजों को आज़माएं।

## ऑफलाइन एक्सेस

आप इस दस्तावेज़ को ऑफलाइन [Docsify](https://docsify.js.org/#/) का उपयोग करके चला सकते हैं। इस रिपॉजिटरी को फोर्क करें, [Docsify इंस्टॉल करें](https://docsify.js.org/#/quickstart) अपने स्थानीय मशीन पर, फिर इस रिपॉजिटरी के रूट फ़ोल्डर में `docsify serve` टाइप करें। वेबसाइट आपके localhost पर पोर्ट 3000 पर सर्व की जाएगी: `localhost:3000`।

> नोट, नोटबुक्स Docsify के माध्यम से रेंडर नहीं किए जाएंगे, इसलिए जब आपको नोटबुक चलाने की आवश्यकता हो, तो इसे अलग से Python कर्नेल चलाते हुए VS Code में करें।

## अन्य पाठ्यक्रम

हमारी टीम अन्य पाठ्यक्रम भी बनाती है! देखें:

- [Generative AI for Beginners](https://aka.ms/genai-beginners)
- [Generative AI for Beginners .NET](https://github.com/microsoft/Generative-AI-for-beginners-dotnet)
- [Generative AI with JavaScript](https://github.com/microsoft/generative-ai-with-javascript)
- [Generative AI with Java](https://aka.ms/genaijava)
- [AI for Beginners](https://aka.ms/ai-beginners)
- [Data Science for Beginners](https://aka.ms/datascience-beginners)
- [Bash for Beginners](https://github.com/microsoft/bash-for-beginners)
- [ML for Beginners](https://aka.ms/ml-beginners)
- [Cybersecurity for Beginners](https://github.com/microsoft/Security-101) 
- [Web Dev for Beginners](https://aka.ms/webdev-beginners)
- [IoT for Beginners](https://aka.ms/iot-beginners)
- [Machine Learning for Beginners](https://aka.ms/ml-beginners)
- [XR Development for Beginners](https://aka.ms/xr-dev-for-beginners)
- [Mastering GitHub Copilot for AI Paired Programming](https://aka.ms/GitHubCopilotAI)
- [XR Development for Beginners](https://github.com/microsoft/xr-development-for-beginners)
- [Mastering GitHub Copilot for C#/.NET Developers](https://github.com/microsoft/mastering-github-copilot-for-dotnet-csharp-developers)
- [Choose Your Own Copilot Adventure](https://github.com/microsoft/CopilotAdventures)

---

