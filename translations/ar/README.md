<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "6bb17a440fdabf0823105136a5b81029",
  "translation_date": "2025-08-27T08:09:13+00:00",
  "source_file": "README.md",
  "language_code": "ar"
}
-->
# علم البيانات للمبتدئين - منهج دراسي

Azure Cloud Advocates في Microsoft يسعدهم تقديم منهج دراسي لمدة 10 أسابيع يتضمن 20 درسًا حول علم البيانات. يحتوي كل درس على اختبارات قبل وبعد الدرس، وتعليمات مكتوبة لإكمال الدرس، وحل، ومهمة. تعتمد طريقتنا التعليمية على المشاريع، مما يتيح لك التعلم أثناء البناء، وهي طريقة مثبتة لجعل المهارات الجديدة "تترسخ".

**شكر خاص لمؤلفينا:** [جاسمين جريناواي](https://www.twitter.com/paladique)، [ديمتري سوشنيكوف](http://soshnikov.com)، [نيتيا ناراسيمهان](https://twitter.com/nitya)، [جيلين ماكجي](https://twitter.com/JalenMcG)، [جين لوبر](https://twitter.com/jenlooper)، [مود ليفي](https://twitter.com/maudstweets)، [تيفاني سوتير](https://twitter.com/TiffanySouterre)، [كريستوفر هاريسون](https://www.twitter.com/geektrainer).

**🙏 شكر خاص 🙏 لـ [سفراء الطلاب في Microsoft](https://studentambassadors.microsoft.com/) المؤلفين، المراجعين، والمساهمين في المحتوى،** ومن بينهم أريان أرورا، [أديتيا جارج](https://github.com/AdityaGarg00)، [ألوندرا سانشيز](https://www.linkedin.com/in/alondra-sanchez-molina/)، [أنكيتا سينغ](https://www.linkedin.com/in/ankitasingh007)، [أنوبام ميشرا](https://www.linkedin.com/in/anupam--mishra/)، [أربيتا داس](https://www.linkedin.com/in/arpitadas01/)، شيل بيهاري دوباي، [ديبري نسوفور](https://www.linkedin.com/in/dibrinsofor)، [ديشيتا بهاسين](https://www.linkedin.com/in/dishita-bhasin-7065281bb)، [مجد صافي](https://www.linkedin.com/in/majd-s/)، [ماكس بلوم](https://www.linkedin.com/in/max-blum-6036a1186/)، [ميغيل كوريا](https://www.linkedin.com/in/miguelmque/)، [محمد افتخار (إفتو) ابن جلال](https://twitter.com/iftu119)، [نورين تبسم](https://www.linkedin.com/in/nawrin-tabassum)، [ريموند وانجسا بوترا](https://www.linkedin.com/in/raymond-wp/)، [روهيت ياداف](https://www.linkedin.com/in/rty2423)، سمردهي شارما، [سانيا سينها](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200)، [شينا نارولا](https://www.linkedin.com/in/sheena-narua-n/)، [توقير أحمد](https://www.linkedin.com/in/tauqeerahmad5201/)، يوغندراسينغ باوار، [فيدوشي جوبتا](https://www.linkedin.com/in/vidushi-gupta07/)، [جسلين سوندي](https://www.linkedin.com/in/jasleen-sondhi/)

|![رسم توضيحي من [(@sketchthedocs)](https://sketchthedocs.dev)](./sketchnotes/00-Title.png)|
|:---:|
| علم البيانات للمبتدئين - _رسم توضيحي من [@nitya](https://twitter.com/nitya)_ |

## إعلان - منهج جديد حول الذكاء الاصطناعي التوليدي تم إصداره للتو!

لقد أصدرنا منهجًا مكونًا من 12 درسًا حول الذكاء الاصطناعي التوليدي. تعال وتعلم أشياء مثل:

- التوجيه وهندسة التوجيه
- إنشاء تطبيقات نصوص وصور
- تطبيقات البحث

كالعادة، هناك درس، مهام لإكمالها، اختبارات معرفية وتحديات.

اطلع عليه:

> https://aka.ms/genai-beginners

# هل أنت طالب؟

ابدأ باستخدام الموارد التالية:

- [صفحة مركز الطلاب](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) ستجد في هذه الصفحة موارد للمبتدئين، حزم الطلاب وحتى طرق للحصول على قسيمة شهادة مجانية. هذه صفحة يجب أن تضيفها إلى إشاراتك المرجعية وتفحصها من وقت لآخر حيث نقوم بتحديث المحتوى شهريًا على الأقل.
- [سفراء الطلاب في Microsoft](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) انضم إلى مجتمع عالمي من سفراء الطلاب، قد تكون هذه فرصتك للدخول إلى Microsoft.

# كيفية البدء

> **للمعلمين**: لقد قمنا [بتضمين بعض الاقتراحات](for-teachers.md) حول كيفية استخدام هذا المنهج. نود أن نسمع ملاحظاتكم [في منتدى النقاش الخاص بنا](https://github.com/microsoft/Data-Science-For-Beginners/discussions)!

> **[للطلاب](https://aka.ms/student-page)**: لاستخدام هذا المنهج بمفردك، قم بعمل fork للمستودع بأكمله وأكمل التمارين بنفسك، بدءًا من اختبار ما قبل المحاضرة. ثم اقرأ المحاضرة وأكمل بقية الأنشطة. حاول إنشاء المشاريع من خلال فهم الدروس بدلاً من نسخ كود الحل؛ ومع ذلك، يتوفر هذا الكود في مجلدات /solutions في كل درس قائم على المشاريع. فكرة أخرى هي تشكيل مجموعة دراسة مع أصدقائك ومراجعة المحتوى معًا. لمزيد من الدراسة، نوصي بـ [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum).

## تعرف على الفريق

[![فيديو ترويجي](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "فيديو ترويجي")

**الرسوم المتحركة بواسطة** [موهيت جايسال](https://www.linkedin.com/in/mohitjaisal)

> 🎥 انقر على الصورة أعلاه لمشاهدة فيديو عن المشروع والأشخاص الذين أنشأوه!

## الطريقة التعليمية

لقد اخترنا مبدأين تعليميين أثناء بناء هذا المنهج: التأكد من أنه قائم على المشاريع وأنه يتضمن اختبارات متكررة. بحلول نهاية هذه السلسلة، سيتعلم الطلاب المبادئ الأساسية لعلم البيانات، بما في ذلك المفاهيم الأخلاقية، إعداد البيانات، طرق مختلفة للعمل مع البيانات، تصور البيانات، تحليل البيانات، حالات استخدام علم البيانات في العالم الحقيقي، والمزيد.

بالإضافة إلى ذلك، يحدد الاختبار منخفض المخاطر قبل الفصل نية الطالب لتعلم موضوع معين، بينما يضمن اختبار آخر بعد الفصل مزيدًا من الاحتفاظ بالمعلومات. تم تصميم هذا المنهج ليكون مرنًا وممتعًا ويمكن تناوله بالكامل أو جزئيًا. تبدأ المشاريع صغيرة وتصبح أكثر تعقيدًا تدريجيًا بحلول نهاية دورة الـ 10 أسابيع.

> اعثر على [مدونة قواعد السلوك](CODE_OF_CONDUCT.md)، [إرشادات المساهمة](CONTRIBUTING.md)، [إرشادات الترجمة](TRANSLATIONS.md). نرحب بملاحظاتكم البناءة!

## يتضمن كل درس:

- رسم توضيحي اختياري
- فيديو إضافي اختياري
- اختبار تمهيدي قبل الدرس
- درس مكتوب
- بالنسبة للدروس القائمة على المشاريع، إرشادات خطوة بخطوة حول كيفية بناء المشروع
- اختبارات معرفية
- تحدٍ
- قراءة إضافية
- مهمة
- اختبار بعد الدرس

> **ملاحظة حول الاختبارات**: جميع الاختبارات موجودة في مجلد Quiz-App، بإجمالي 40 اختبارًا يحتوي كل منها على ثلاثة أسئلة. يتم ربطها من داخل الدروس، ولكن يمكن تشغيل تطبيق الاختبار محليًا أو نشره على Azure؛ اتبع التعليمات في مجلد `quiz-app`. يتم ترجمتها تدريجيًا.

## الدروس

|![رسم توضيحي من [(@sketchthedocs)](https://sketchthedocs.dev)](./sketchnotes/00-Roadmap.png)|
|:---:|
| علم البيانات للمبتدئين: خارطة الطريق - _رسم توضيحي من [@nitya](https://twitter.com/nitya)_ |

| رقم الدرس | الموضوع | مجموعة الدروس | أهداف التعلم | الدرس المرتبط | المؤلف |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | تعريف علم البيانات | [المقدمة](1-Introduction/README.md) | تعلم المفاهيم الأساسية وراء علم البيانات وكيف يرتبط بالذكاء الاصطناعي، التعلم الآلي، والبيانات الضخمة. | [الدرس](1-Introduction/01-defining-data-science/README.md) [الفيديو](https://youtu.be/beZ7Mb_oz9I) | [ديمتري](http://soshnikov.com) |
| 02 | أخلاقيات علم البيانات | [المقدمة](1-Introduction/README.md) | مفاهيم أخلاقيات البيانات، التحديات والأطر. | [الدرس](1-Introduction/02-ethics/README.md) | [نيتيا](https://twitter.com/nitya) |
| 03 | تعريف البيانات | [المقدمة](1-Introduction/README.md) | كيفية تصنيف البيانات ومصادرها الشائعة. | [الدرس](1-Introduction/03-defining-data/README.md) | [جاسمين](https://www.twitter.com/paladique) |
| 04 | مقدمة في الإحصاء والاحتمالات | [المقدمة](1-Introduction/README.md) | التقنيات الرياضية للاحتمالات والإحصاء لفهم البيانات. | [الدرس](1-Introduction/04-stats-and-probability/README.md) [الفيديو](https://youtu.be/Z5Zy85g4Yjw) | [ديمتري](http://soshnikov.com) |
| 05 | العمل مع البيانات العلائقية | [العمل مع البيانات](2-Working-With-Data/README.md) | مقدمة في البيانات العلائقية وأساسيات استكشاف وتحليل البيانات العلائقية باستخدام لغة الاستعلام الهيكلية، المعروفة أيضًا بـ SQL (تُنطق "سي-كويل"). | [الدرس](2-Working-With-Data/05-relational-databases/README.md) | [كريستوفر](https://www.twitter.com/geektrainer) |
| 06 | العمل مع بيانات NoSQL | [العمل مع البيانات](2-Working-With-Data/README.md) | مقدمة في البيانات غير العلائقية، أنواعها المختلفة وأساسيات استكشاف وتحليل قواعد بيانات الوثائق. | [الدرس](2-Working-With-Data/06-non-relational/README.md) | [جاسمين](https://twitter.com/paladique) |
| 07 | العمل مع بايثون | [العمل مع البيانات](2-Working-With-Data/README.md) | أساسيات استخدام بايثون لاستكشاف البيانات باستخدام مكتبات مثل Pandas. يُفضل وجود فهم أساسي لبرمجة بايثون. | [الدرس](2-Working-With-Data/07-python/README.md) [الفيديو](https://youtu.be/dZjWOGbsN4Y) | [ديمتري](http://soshnikov.com) |
| 08 | إعداد البيانات | [العمل مع البيانات](2-Working-With-Data/README.md) | مواضيع حول تقنيات تنظيف وتحويل البيانات للتعامل مع تحديات البيانات المفقودة أو غير الدقيقة أو غير المكتملة. | [الدرس](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | تصور الكميات | [تصور البيانات](3-Data-Visualization/README.md) | تعلم كيفية استخدام Matplotlib لتصور بيانات الطيور 🦆 | [الدرس](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | تصور توزيع البيانات | [تصور البيانات](3-Data-Visualization/README.md) | تصور الملاحظات والاتجاهات ضمن فترة زمنية. | [الدرس](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | تصور النسب | [تصور البيانات](3-Data-Visualization/README.md) | تصور النسب المئوية المنفصلة والمجمعة. | [الدرس](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | تصور العلاقات | [تصور البيانات](3-Data-Visualization/README.md) | تصور الروابط والارتباطات بين مجموعات البيانات ومتغيراتها. | [الدرس](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | تصورات ذات معنى | [تصور البيانات](3-Data-Visualization/README.md) | تقنيات وإرشادات لجعل تصوراتك ذات قيمة لحل المشكلات بشكل فعال واستخلاص الأفكار. | [الدرس](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | مقدمة في دورة حياة علم البيانات | [دورة الحياة](4-Data-Science-Lifecycle/README.md) | مقدمة في دورة حياة علم البيانات وخطوتها الأولى في الحصول على البيانات واستخراجها. | [الدرس](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | التحليل | [دورة الحياة](4-Data-Science-Lifecycle/README.md) | تركز هذه المرحلة من دورة حياة علم البيانات على تقنيات تحليل البيانات. | [الدرس](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | التواصل | [دورة الحياة](4-Data-Science-Lifecycle/README.md) | تركز هذه المرحلة من دورة حياة علم البيانات على تقديم الأفكار المستخلصة من البيانات بطريقة تسهل على صناع القرار فهمها. | [الدرس](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | علم البيانات في السحابة | [بيانات السحابة](5-Data-Science-In-Cloud/README.md) | تقدم هذه السلسلة من الدروس علم البيانات في السحابة وفوائده. | [الدرس](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) و [Maud](https://twitter.com/maudstweets) |
| 18 | علم البيانات في السحابة | [بيانات السحابة](5-Data-Science-In-Cloud/README.md) | تدريب النماذج باستخدام أدوات Low Code. | [الدرس](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) و [Maud](https://twitter.com/maudstweets) |
| 19 | علم البيانات في السحابة | [بيانات السحابة](5-Data-Science-In-Cloud/README.md) | نشر النماذج باستخدام Azure Machine Learning Studio. | [الدرس](5-Data-Science-In-Cloud/19-Azure/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) و [Maud](https://twitter.com/maudstweets) |
| 20 | علم البيانات في العالم الحقيقي | [في العالم الحقيقي](6-Data-Science-In-Wild/README.md) | مشاريع علم البيانات المدفوعة في العالم الحقيقي. | [الدرس](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

اتبع هذه الخطوات لفتح هذا المثال في Codespace:
1. انقر على القائمة المنسدلة "Code" واختر خيار "Open with Codespaces".
2. اختر + New codespace في أسفل اللوحة.
لمزيد من المعلومات، تحقق من [وثائق GitHub](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace).

## VSCode Remote - Containers
اتبع هذه الخطوات لفتح هذا المستودع في حاوية باستخدام جهازك المحلي وVSCode باستخدام امتداد VS Code Remote - Containers:

1. إذا كانت هذه هي المرة الأولى التي تستخدم فيها حاوية تطوير، يرجى التأكد من أن نظامك يلبي المتطلبات الأساسية (مثل تثبيت Docker) في [وثائق البدء](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started).

لاستخدام هذا المستودع، يمكنك فتحه إما في وحدة تخزين Docker معزولة:

**ملاحظة**: في الخلفية، سيتم استخدام أمر Remote-Containers: **Clone Repository in Container Volume...** لنسخ الكود المصدر في وحدة تخزين Docker بدلاً من نظام الملفات المحلي. [الوحدات التخزينية](https://docs.docker.com/storage/volumes/) هي الآلية المفضلة للحفاظ على بيانات الحاوية.

أو فتح نسخة محلية مستنسخة أو محملة من المستودع:

- قم باستنساخ هذا المستودع إلى نظام الملفات المحلي.
- اضغط F1 واختر الأمر **Remote-Containers: Open Folder in Container...**.
- اختر النسخة المستنسخة من هذا المجلد، انتظر حتى تبدأ الحاوية، وجرب الأمور.

## الوصول دون اتصال

يمكنك تشغيل هذا التوثيق دون اتصال باستخدام [Docsify](https://docsify.js.org/#/). قم باستنساخ هذا المستودع، [تثبيت Docsify](https://docsify.js.org/#/quickstart) على جهازك المحلي، ثم في المجلد الجذري لهذا المستودع، اكتب `docsify serve`. سيتم تقديم الموقع على المنفذ 3000 على localhost: `localhost:3000`.

> ملاحظة، لن يتم عرض دفاتر الملاحظات عبر Docsify، لذا عندما تحتاج إلى تشغيل دفتر ملاحظات، قم بذلك بشكل منفصل في VS Code باستخدام نواة Python.

## مطلوب مساعدة!

إذا كنت ترغب في ترجمة كل أو جزء من المنهج، يرجى اتباع دليلنا [Translations](TRANSLATIONS.md).

## مناهج أخرى

فريقنا ينتج مناهج أخرى! تحقق من:

- [الذكاء الاصطناعي التوليدي للمبتدئين](https://aka.ms/genai-beginners)
- [الذكاء الاصطناعي التوليدي للمبتدئين .NET](https://github.com/microsoft/Generative-AI-for-beginners-dotnet)
- [الذكاء الاصطناعي التوليدي باستخدام JavaScript](https://github.com/microsoft/generative-ai-with-javascript)
- [الذكاء الاصطناعي التوليدي باستخدام Java](https://aka.ms/genaijava)
- [الذكاء الاصطناعي للمبتدئين](https://aka.ms/ai-beginners)
- [علم البيانات للمبتدئين](https://aka.ms/datascience-beginners)
- [تعلم الآلة للمبتدئين](https://aka.ms/ml-beginners)
- [الأمن السيبراني للمبتدئين](https://github.com/microsoft/Security-101) 
- [تطوير الويب للمبتدئين](https://aka.ms/webdev-beginners)
- [إنترنت الأشياء للمبتدئين](https://aka.ms/iot-beginners)
- [تطوير الواقع الممتد للمبتدئين](https://github.com/microsoft/xr-development-for-beginners)
- [إتقان GitHub Copilot للبرمجة الزوجية](https://github.com/microsoft/Mastering-GitHub-Copilot-for-Paired-Programming)
- [إتقان GitHub Copilot لمطوري C#/.NET](https://github.com/microsoft/mastering-github-copilot-for-dotnet-csharp-developers)
- [اختر مغامرتك مع Copilot](https://github.com/microsoft/CopilotAdventures)

---

**إخلاء المسؤولية**:  
تمت ترجمة هذا المستند باستخدام خدمة الترجمة الآلية [Co-op Translator](https://github.com/Azure/co-op-translator). بينما نسعى لتحقيق الدقة، يرجى العلم أن الترجمات الآلية قد تحتوي على أخطاء أو معلومات غير دقيقة. يجب اعتبار المستند الأصلي بلغته الأصلية هو المصدر الموثوق. للحصول على معلومات حساسة أو هامة، يُوصى بالاستعانة بترجمة بشرية احترافية. نحن غير مسؤولين عن أي سوء فهم أو تفسيرات خاطئة تنشأ عن استخدام هذه الترجمة.