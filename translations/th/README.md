<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "f9a704f7494ca2d185ded59ba3da99ef",
  "translation_date": "2025-10-24T09:10:13+00:00",
  "source_file": "README.md",
  "language_code": "th"
}
-->
# วิทยาศาสตร์ข้อมูลสำหรับผู้เริ่มต้น - หลักสูตร

Azure Cloud Advocates ที่ Microsoft ยินดีนำเสนอหลักสูตร 10 สัปดาห์ 20 บทเรียนเกี่ยวกับวิทยาศาสตร์ข้อมูล แต่ละบทเรียนประกอบด้วยแบบทดสอบก่อนและหลังบทเรียน คำแนะนำที่เขียนไว้เพื่อทำบทเรียนให้สำเร็จ โซลูชัน และงานมอบหมาย วิธีการเรียนรู้แบบโครงการช่วยให้คุณเรียนรู้ผ่านการสร้าง ซึ่งเป็นวิธีที่พิสูจน์แล้วว่าทักษะใหม่จะติดตัวคุณได้ดี

**ขอขอบคุณผู้เขียนของเรา:** [Jasmine Greenaway](https://www.twitter.com/paladique), [Dmitry Soshnikov](http://soshnikov.com), [Nitya Narasimhan](https://twitter.com/nitya), [Jalen McGee](https://twitter.com/JalenMcG), [Jen Looper](https://twitter.com/jenlooper), [Maud Levy](https://twitter.com/maudstweets), [Tiffany Souterre](https://twitter.com/TiffanySouterre), [Christopher Harrison](https://www.twitter.com/geektrainer).

**🙏 ขอบคุณพิเศษ 🙏 สำหรับ [Microsoft Student Ambassador](https://studentambassadors.microsoft.com/) ผู้เขียน ผู้ตรวจสอบ และผู้มีส่วนร่วมในเนื้อหา,** โดยเฉพาะ Aaryan Arora, [Aditya Garg](https://github.com/AdityaGarg00), [Alondra Sanchez](https://www.linkedin.com/in/alondra-sanchez-molina/), [Ankita Singh](https://www.linkedin.com/in/ankitasingh007), [Anupam Mishra](https://www.linkedin.com/in/anupam--mishra/), [Arpita Das](https://www.linkedin.com/in/arpitadas01/), ChhailBihari Dubey, [Dibri Nsofor](https://www.linkedin.com/in/dibrinsofor), [Dishita Bhasin](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [Majd Safi](https://www.linkedin.com/in/majd-s/), [Max Blum](https://www.linkedin.com/in/max-blum-6036a1186/), [Miguel Correa](https://www.linkedin.com/in/miguelmque/), [Mohamma Iftekher (Iftu) Ebne Jalal](https://twitter.com/iftu119), [Nawrin Tabassum](https://www.linkedin.com/in/nawrin-tabassum), [Raymond Wangsa Putra](https://www.linkedin.com/in/raymond-wp/), [Rohit Yadav](https://www.linkedin.com/in/rty2423), Samridhi Sharma, [Sanya Sinha](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200),
[Sheena Narula](https://www.linkedin.com/in/sheena-narua-n/), [Tauqeer Ahmad](https://www.linkedin.com/in/tauqeerahmad5201/), Yogendrasingh Pawar , [Vidushi Gupta](https://www.linkedin.com/in/vidushi-gupta07/), [Jasleen Sondhi](https://www.linkedin.com/in/jasleen-sondhi/)

|![ภาพสเก็ตโน้ตโดย @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.th.png)|
|:---:|
| วิทยาศาสตร์ข้อมูลสำหรับผู้เริ่มต้น - _ภาพสเก็ตโน้ตโดย [@nitya](https://twitter.com/nitya)_ |

### 🌐 การสนับสนุนหลายภาษา

#### รองรับผ่าน GitHub Action (อัตโนมัติและอัปเดตเสมอ)

[Arabic](../ar/README.md) | [Bengali](../bn/README.md) | [Bulgarian](../bg/README.md) | [Burmese (Myanmar)](../my/README.md) | [Chinese (Simplified)](../zh/README.md) | [Chinese (Traditional, Hong Kong)](../hk/README.md) | [Chinese (Traditional, Macau)](../mo/README.md) | [Chinese (Traditional, Taiwan)](../tw/README.md) | [Croatian](../hr/README.md) | [Czech](../cs/README.md) | [Danish](../da/README.md) | [Dutch](../nl/README.md) | [Estonian](../et/README.md) | [Finnish](../fi/README.md) | [French](../fr/README.md) | [German](../de/README.md) | [Greek](../el/README.md) | [Hebrew](../he/README.md) | [Hindi](../hi/README.md) | [Hungarian](../hu/README.md) | [Indonesian](../id/README.md) | [Italian](../it/README.md) | [Japanese](../ja/README.md) | [Korean](../ko/README.md) | [Lithuanian](../lt/README.md) | [Malay](../ms/README.md) | [Marathi](../mr/README.md) | [Nepali](../ne/README.md) | [Norwegian](../no/README.md) | [Persian (Farsi)](../fa/README.md) | [Polish](../pl/README.md) | [Portuguese (Brazil)](../br/README.md) | [Portuguese (Portugal)](../pt/README.md) | [Punjabi (Gurmukhi)](../pa/README.md) | [Romanian](../ro/README.md) | [Russian](../ru/README.md) | [Serbian (Cyrillic)](../sr/README.md) | [Slovak](../sk/README.md) | [Slovenian](../sl/README.md) | [Spanish](../es/README.md) | [Swahili](../sw/README.md) | [Swedish](../sv/README.md) | [Tagalog (Filipino)](../tl/README.md) | [Tamil](../ta/README.md) | [Thai](./README.md) | [Turkish](../tr/README.md) | [Ukrainian](../uk/README.md) | [Urdu](../ur/README.md) | [Vietnamese](../vi/README.md)

**หากคุณต้องการให้มีการสนับสนุนการแปลเพิ่มเติม รายการภาษาที่รองรับอยู่ [ที่นี่](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md)**

#### เข้าร่วมชุมชนของเรา 
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://aka.ms/ds4beginners/discord)

เรามีซีรีส์เรียนรู้กับ AI ใน Discord ที่กำลังดำเนินการอยู่ เรียนรู้เพิ่มเติมและเข้าร่วมกับเราได้ที่ [Learn with AI Series](https://aka.ms/learnwithai/discord) ตั้งแต่วันที่ 18 - 30 กันยายน 2025 คุณจะได้รับเคล็ดลับและเทคนิคในการใช้ GitHub Copilot สำหรับวิทยาศาสตร์ข้อมูล

![ซีรีส์เรียนรู้กับ AI](../../translated_images/1.2b28cdc6205e26fef6a21817fe5d83ae8b50fbd0a33e9fed0df05845da5b30b6.th.jpg)

# คุณเป็นนักเรียนหรือไม่?

เริ่มต้นด้วยทรัพยากรต่อไปนี้:

- [หน้าศูนย์นักเรียน](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) ในหน้านี้ คุณจะพบทรัพยากรสำหรับผู้เริ่มต้น ชุดนักเรียน และแม้กระทั่งวิธีการรับบัตรรับรองฟรี นี่คือหน้าที่คุณควรบันทึกไว้และตรวจสอบเป็นระยะๆ เนื่องจากเรามีการเปลี่ยนแปลงเนื้อหาอย่างน้อยเดือนละครั้ง
- [Microsoft Learn Student Ambassadors](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) เข้าร่วมชุมชนระดับโลกของนักเรียนทูต นี่อาจเป็นทางเข้าสู่ Microsoft ของคุณ

# เริ่มต้นใช้งาน

## 📚 เอกสาร

- **[คู่มือการติดตั้ง](INSTALLATION.md)** - คำแนะนำการตั้งค่าแบบทีละขั้นตอนสำหรับผู้เริ่มต้น
- **[คู่มือการใช้งาน](USAGE.md)** - ตัวอย่างและกระบวนการทำงานทั่วไป
- **[การแก้ไขปัญหา](TROUBLESHOOTING.md)** - วิธีแก้ไขปัญหาทั่วไป
- **[คู่มือการมีส่วนร่วม](CONTRIBUTING.md)** - วิธีการมีส่วนร่วมในโครงการนี้
- **[สำหรับครู](for-teachers.md)** - คำแนะนำการสอนและทรัพยากรในห้องเรียน

## 👨‍🎓 สำหรับนักเรียน
> **ผู้เริ่มต้นทั้งหมด**: ใหม่กับวิทยาศาสตร์ข้อมูล? เริ่มต้นด้วย [ตัวอย่างที่เหมาะสำหรับผู้เริ่มต้น](examples/README.md)! ตัวอย่างที่เรียบง่ายและมีคำอธิบายเหล่านี้จะช่วยให้คุณเข้าใจพื้นฐานก่อนที่จะเข้าสู่หลักสูตรเต็มรูปแบบ
> **[นักเรียน](https://aka.ms/student-page)**: เพื่อใช้หลักสูตรนี้ด้วยตัวเอง ให้ fork repo ทั้งหมดและทำแบบฝึกหัดด้วยตัวเอง โดยเริ่มต้นด้วยแบบทดสอบก่อนการบรรยาย จากนั้นอ่านการบรรยายและทำกิจกรรมที่เหลือ พยายามสร้างโครงการโดยการเข้าใจบทเรียนแทนที่จะคัดลอกรหัสโซลูชัน อย่างไรก็ตาม รหัสนั้นมีอยู่ในโฟลเดอร์ /solutions ในแต่ละบทเรียนที่เน้นโครงการ อีกแนวคิดหนึ่งคือการสร้างกลุ่มศึกษาและเรียนรู้เนื้อหาด้วยกัน สำหรับการศึกษาเพิ่มเติม เราแนะนำ [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum)

**เริ่มต้นอย่างรวดเร็ว:**
1. ตรวจสอบ [คู่มือการติดตั้ง](INSTALLATION.md) เพื่อเตรียมสภาพแวดล้อมของคุณ
2. ทบทวน [คู่มือการใช้งาน](USAGE.md) เพื่อเรียนรู้วิธีการทำงานกับหลักสูตร
3. เริ่มต้นด้วยบทเรียนที่ 1 และทำตามลำดับ
4. เข้าร่วมชุมชน [Discord ของเรา](https://aka.ms/ds4beginners/discord) เพื่อรับการสนับสนุน

## 👩‍🏫 สำหรับครู

> **ครู**: เราได้ [รวมคำแนะนำบางส่วน](for-teachers.md) เกี่ยวกับวิธีการใช้หลักสูตรนี้ เราอยากได้รับความคิดเห็นของคุณ [ในฟอรัมการสนทนาของเรา](https://github.com/microsoft/Data-Science-For-Beginners/discussions)!

## พบกับทีมงาน

[![วิดีโอโปรโมต](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "วิดีโอโปรโมต")

**Gif โดย** [Mohit Jaisal](https://www.linkedin.com/in/mohitjaisal)

> 🎥 คลิกที่ภาพด้านบนเพื่อดูวิดีโอเกี่ยวกับโครงการและผู้ที่สร้างมันขึ้นมา!

## วิธีการสอน
เราได้เลือกหลักการการสอนสองข้อในการสร้างหลักสูตรนี้: การทำให้เป็นโครงการและการมีแบบทดสอบบ่อยครั้ง เมื่อจบหลักสูตรนี้ นักเรียนจะได้เรียนรู้หลักการพื้นฐานของวิทยาศาสตร์ข้อมูล รวมถึงแนวคิดด้านจริยธรรม การเตรียมข้อมูล วิธีการทำงานกับข้อมูล การสร้างภาพข้อมูล การวิเคราะห์ข้อมูล กรณีการใช้งานจริงของวิทยาศาสตร์ข้อมูล และอื่นๆ

นอกจากนี้ แบบทดสอบที่มีความเสี่ยงต่ำก่อนเริ่มเรียนจะช่วยให้นักเรียนตั้งเป้าหมายในการเรียนรู้หัวข้อ และแบบทดสอบหลังเรียนจะช่วยเสริมความจำ หลักสูตรนี้ถูกออกแบบให้มีความยืดหยุ่นและสนุกสนาน สามารถเรียนได้ทั้งแบบเต็มหลักสูตรหรือบางส่วน โครงการเริ่มต้นจากง่ายและซับซ้อนขึ้นเรื่อยๆ ในช่วง 10 สัปดาห์

> ดู [Code of Conduct](CODE_OF_CONDUCT.md), [Contributing](CONTRIBUTING.md), [Translation](TRANSLATIONS.md) guidelines เรายินดีรับฟังความคิดเห็นที่สร้างสรรค์ของคุณ!

## แต่ละบทเรียนประกอบด้วย:

- ภาพสเก็ตช์โน้ต (ตัวเลือก)
- วิดีโอเสริม (ตัวเลือก)
- แบบทดสอบอุ่นเครื่องก่อนบทเรียน
- บทเรียนที่เขียนขึ้น
- สำหรับบทเรียนที่เน้นโครงการ มีคำแนะนำทีละขั้นตอนในการสร้างโครงการ
- การตรวจสอบความรู้
- ความท้าทาย
- การอ่านเสริม
- งานที่มอบหมาย
- [แบบทดสอบหลังบทเรียน](https://ff-quizzes.netlify.app/en/)

> **หมายเหตุเกี่ยวกับแบบทดสอบ**: แบบทดสอบทั้งหมดอยู่ในโฟลเดอร์ Quiz-App มีทั้งหมด 40 แบบทดสอบ แต่ละแบบมี 3 คำถาม แบบทดสอบเหล่านี้เชื่อมโยงจากบทเรียน แต่แอปแบบทดสอบสามารถรันได้ในเครื่องหรือปรับใช้บน Azure โดยทำตามคำแนะนำในโฟลเดอร์ `quiz-app` แบบทดสอบกำลังถูกแปลเป็นภาษาต่างๆ อย่างต่อเนื่อง

## 🎓 ตัวอย่างที่เหมาะสำหรับผู้เริ่มต้น

**ใหม่กับวิทยาศาสตร์ข้อมูล?** เราได้สร้าง [ไดเรกทอรีตัวอย่าง](examples/README.md) ที่มีโค้ดง่ายๆ พร้อมคำอธิบายเพื่อช่วยให้คุณเริ่มต้น:

- 🌟 **Hello World** - โปรแกรมวิทยาศาสตร์ข้อมูลแรกของคุณ
- 📂 **การโหลดข้อมูล** - เรียนรู้การอ่านและสำรวจชุดข้อมูล
- 📊 **การวิเคราะห์ง่ายๆ** - คำนวณสถิติและค้นหารูปแบบ
- 📈 **การสร้างภาพพื้นฐาน** - สร้างแผนภูมิและกราฟ
- 🔬 **โครงการในโลกจริง** - กระบวนการทำงานตั้งแต่ต้นจนจบ

ตัวอย่างแต่ละตัวมีคำอธิบายรายละเอียดในทุกขั้นตอน เหมาะสำหรับผู้เริ่มต้นอย่างแท้จริง!

👉 **[เริ่มต้นด้วยตัวอย่าง](examples/README.md)** 👈

## บทเรียน


|![ Sketchnote by @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.th.png)|
|:---:|
| วิทยาศาสตร์ข้อมูลสำหรับผู้เริ่มต้น: แผนที่เส้นทาง - _ภาพสเก็ตช์โน้ตโดย [@nitya](https://twitter.com/nitya)_ |


| หมายเลขบทเรียน | หัวข้อ | กลุ่มบทเรียน | วัตถุประสงค์การเรียนรู้ | ลิงก์บทเรียน | ผู้เขียน |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | การนิยามวิทยาศาสตร์ข้อมูล | [บทนำ](1-Introduction/README.md) | เรียนรู้แนวคิดพื้นฐานของวิทยาศาสตร์ข้อมูลและความสัมพันธ์กับปัญญาประดิษฐ์ การเรียนรู้ของเครื่อง และข้อมูลขนาดใหญ่ | [บทเรียน](1-Introduction/01-defining-data-science/README.md) [วิดีโอ](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | จริยธรรมในวิทยาศาสตร์ข้อมูล | [บทนำ](1-Introduction/README.md) | แนวคิดด้านจริยธรรมในข้อมูล ความท้าทาย และกรอบการทำงาน | [บทเรียน](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | การนิยามข้อมูล | [บทนำ](1-Introduction/README.md) | วิธีการจัดประเภทข้อมูลและแหล่งข้อมูลทั่วไป | [บทเรียน](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | บทนำสู่สถิติและความน่าจะเป็น | [บทนำ](1-Introduction/README.md) | เทคนิคทางคณิตศาสตร์ของความน่าจะเป็นและสถิติในการทำความเข้าใจข้อมูล | [บทเรียน](1-Introduction/04-stats-and-probability/README.md) [วิดีโอ](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | การทำงานกับข้อมูลเชิงสัมพันธ์ | [การทำงานกับข้อมูล](2-Working-With-Data/README.md) | บทนำสู่ข้อมูลเชิงสัมพันธ์และพื้นฐานการสำรวจและวิเคราะห์ข้อมูลเชิงสัมพันธ์ด้วย Structured Query Language หรือ SQL | [บทเรียน](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | การทำงานกับข้อมูล NoSQL | [การทำงานกับข้อมูล](2-Working-With-Data/README.md) | บทนำสู่ข้อมูลที่ไม่ใช่เชิงสัมพันธ์ ประเภทต่างๆ และพื้นฐานการสำรวจและวิเคราะห์ฐานข้อมูลเอกสาร | [บทเรียน](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | การทำงานกับ Python | [การทำงานกับข้อมูล](2-Working-With-Data/README.md) | พื้นฐานการใช้ Python ในการสำรวจข้อมูลด้วยไลบรารี เช่น Pandas แนะนำให้มีความเข้าใจพื้นฐานเกี่ยวกับการเขียนโปรแกรม Python | [บทเรียน](2-Working-With-Data/07-python/README.md) [วิดีโอ](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | การเตรียมข้อมูล | [การทำงานกับข้อมูล](2-Working-With-Data/README.md) | หัวข้อเกี่ยวกับเทคนิคการทำความสะอาดและแปลงข้อมูลเพื่อจัดการกับปัญหาข้อมูลที่ขาดหาย ไม่ถูกต้อง หรือไม่สมบูรณ์ | [บทเรียน](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | การสร้างภาพปริมาณข้อมูล | [การสร้างภาพข้อมูล](3-Data-Visualization/README.md) | เรียนรู้การใช้ Matplotlib ในการสร้างภาพข้อมูลนก 🦆 | [บทเรียน](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | การสร้างภาพการกระจายตัวของข้อมูล | [การสร้างภาพข้อมูล](3-Data-Visualization/README.md) | การสร้างภาพการสังเกตและแนวโน้มภายในช่วง | [บทเรียน](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | การสร้างภาพสัดส่วน | [การสร้างภาพข้อมูล](3-Data-Visualization/README.md) | การสร้างภาพเปอร์เซ็นต์แบบแยกและแบบกลุ่ม | [บทเรียน](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | การสร้างภาพความสัมพันธ์ | [การสร้างภาพข้อมูล](3-Data-Visualization/README.md) | การสร้างภาพการเชื่อมโยงและความสัมพันธ์ระหว่างชุดข้อมูลและตัวแปร | [บทเรียน](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | การสร้างภาพที่มีความหมาย | [การสร้างภาพข้อมูล](3-Data-Visualization/README.md) | เทคนิคและคำแนะนำในการทำให้การสร้างภาพของคุณมีคุณค่าเพื่อการแก้ปัญหาและการวิเคราะห์ที่มีประสิทธิภาพ | [บทเรียน](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | บทนำสู่วงจรชีวิตของวิทยาศาสตร์ข้อมูล | [วงจรชีวิต](4-Data-Science-Lifecycle/README.md) | บทนำสู่วงจรชีวิตของวิทยาศาสตร์ข้อมูลและขั้นตอนแรกในการรวบรวมและดึงข้อมูล | [บทเรียน](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | การวิเคราะห์ | [วงจรชีวิต](4-Data-Science-Lifecycle/README.md) | ขั้นตอนนี้ในวงจรชีวิตของวิทยาศาสตร์ข้อมูลมุ่งเน้นไปที่เทคนิคการวิเคราะห์ข้อมูล | [บทเรียน](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | การสื่อสาร | [วงจรชีวิต](4-Data-Science-Lifecycle/README.md) | ขั้นตอนนี้ในวงจรชีวิตของวิทยาศาสตร์ข้อมูลมุ่งเน้นไปที่การนำเสนอข้อมูลเชิงลึกจากข้อมูลในรูปแบบที่ช่วยให้ผู้ตัดสินใจเข้าใจได้ง่ายขึ้น | [บทเรียน](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | วิทยาศาสตร์ข้อมูลในระบบคลาวด์ | [ข้อมูลในคลาวด์](5-Data-Science-In-Cloud/README.md) | บทเรียนชุดนี้แนะนำวิทยาศาสตร์ข้อมูลในระบบคลาวด์และประโยชน์ของมัน | [บทเรียน](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) และ [Maud](https://twitter.com/maudstweets) |
| 18 | วิทยาศาสตร์ข้อมูลในระบบคลาวด์ | [ข้อมูลในคลาวด์](5-Data-Science-In-Cloud/README.md) | การฝึกอบรมโมเดลโดยใช้เครื่องมือ Low Code |[บทเรียน](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) และ [Maud](https://twitter.com/maudstweets) |
| 19 | วิทยาศาสตร์ข้อมูลในระบบคลาวด์ | [ข้อมูลในคลาวด์](5-Data-Science-In-Cloud/README.md) | การปรับใช้โมเดลด้วย Azure Machine Learning Studio | [บทเรียน](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) และ [Maud](https://twitter.com/maudstweets) |
| 20 | วิทยาศาสตร์ข้อมูลในโลกจริง | [ในโลกจริง](6-Data-Science-In-Wild/README.md) | โครงการที่ขับเคลื่อนด้วยวิทยาศาสตร์ข้อมูลในโลกจริง | [บทเรียน](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

ทำตามขั้นตอนเหล่านี้เพื่อเปิดตัวอย่างนี้ใน Codespace:
1. คลิกเมนูดรอปดาวน์ Code และเลือกตัวเลือก Open with Codespaces
2. เลือก + New codespace ที่ด้านล่างของแผง
สำหรับข้อมูลเพิ่มเติม ดู [เอกสาร GitHub](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace).

## VSCode Remote - Containers
ทำตามขั้นตอนเหล่านี้เพื่อเปิด repo นี้ใน container โดยใช้เครื่องของคุณและ VSCode ด้วยส่วนขยาย VS Code Remote - Containers:

1. หากนี่เป็นครั้งแรกที่คุณใช้ container สำหรับการพัฒนา โปรดตรวจสอบให้แน่ใจว่าระบบของคุณตรงตามข้อกำหนดเบื้องต้น (เช่น ติดตั้ง Docker) ใน [เอกสารเริ่มต้น](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started).

ในการใช้ repo นี้ คุณสามารถเปิด repo ใน Docker volume ที่แยกออกมา:

**หมายเหตุ**: ภายใต้การทำงานนี้จะใช้คำสั่ง Remote-Containers: **Clone Repository in Container Volume...** เพื่อโคลนซอร์สโค้ดใน Docker volume แทนที่จะเป็นระบบไฟล์ในเครื่อง [Volumes](https://docs.docker.com/storage/volumes/) เป็นกลไกที่แนะนำสำหรับการเก็บข้อมูล container

หรือเปิดเวอร์ชันที่โคลนหรือดาวน์โหลดไว้ในเครื่อง:

- โคลน repo นี้ไปยังระบบไฟล์ในเครื่องของคุณ
- กด F1 และเลือกคำสั่ง **Remote-Containers: Open Folder in Container...**
- เลือกสำเนาที่โคลนของโฟลเดอร์นี้ รอให้ container เริ่มต้น และลองใช้งาน

## การเข้าถึงแบบออฟไลน์

คุณสามารถรันเอกสารนี้แบบออฟไลน์โดยใช้ [Docsify](https://docsify.js.org/#/). Fork repo นี้, [ติดตั้ง Docsify](https://docsify.js.org/#/quickstart) บนเครื่องของคุณ จากนั้นในโฟลเดอร์ root ของ repo นี้ พิมพ์ `docsify serve`. เว็บไซต์จะถูกให้บริการบนพอร์ต 3000 บน localhost: `localhost:3000`.

> หมายเหตุ โน้ตบุ๊กจะไม่ถูกแสดงผลผ่าน Docsify ดังนั้นเมื่อคุณต้องการรันโน้ตบุ๊ก ให้ทำแยกต่างหากใน VS Code โดยใช้ Python kernel

## หลักสูตรอื่นๆ

ทีมของเราผลิตหลักสูตรอื่นๆ! ดูที่:

<!-- CO-OP TRANSLATOR OTHER COURSES START -->
### Azure / Edge / MCP / Agents
[![AZD for Beginners](https://img.shields.io/badge/AZD%20for%20Beginners-0078D4?style=for-the-badge&labelColor=E5E7EB&color=0078D4)](https://github.com/microsoft/AZD-for-beginners?WT.mc_id=academic-105485-koreyst)
[![Edge AI for Beginners](https://img.shields.io/badge/Edge%20AI%20for%20Beginners-00B8E4?style=for-the-badge&labelColor=E5E7EB&color=00B8E4)](https://github.com/microsoft/edgeai-for-beginners?WT.mc_id=academic-105485-koreyst)
[![MCP สำหรับผู้เริ่มต้น](https://img.shields.io/badge/MCP%20for%20Beginners-009688?style=for-the-badge&labelColor=E5E7EB&color=009688)](https://github.com/microsoft/mcp-for-beginners?WT.mc_id=academic-105485-koreyst)  
[![AI Agents สำหรับผู้เริ่มต้น](https://img.shields.io/badge/AI%20Agents%20for%20Beginners-00C49A?style=for-the-badge&labelColor=E5E7EB&color=00C49A)](https://github.com/microsoft/ai-agents-for-beginners?WT.mc_id=academic-105485-koreyst)

---

### ซีรีส์ Generative AI  
[![Generative AI สำหรับผู้เริ่มต้น](https://img.shields.io/badge/Generative%20AI%20for%20Beginners-8B5CF6?style=for-the-badge&labelColor=E5E7EB&color=8B5CF6)](https://github.com/microsoft/generative-ai-for-beginners?WT.mc_id=academic-105485-koreyst)  
[![Generative AI (.NET)](https://img.shields.io/badge/Generative%20AI%20(.NET)-9333EA?style=for-the-badge&labelColor=E5E7EB&color=9333EA)](https://github.com/microsoft/Generative-AI-for-beginners-dotnet?WT.mc_id=academic-105485-koreyst)  
[![Generative AI (Java)](https://img.shields.io/badge/Generative%20AI%20(Java)-C084FC?style=for-the-badge&labelColor=E5E7EB&color=C084FC)](https://github.com/microsoft/generative-ai-for-beginners-java?WT.mc_id=academic-105485-koreyst)  
[![Generative AI (JavaScript)](https://img.shields.io/badge/Generative%20AI%20(JavaScript)-E879F9?style=for-the-badge&labelColor=E5E7EB&color=E879F9)](https://github.com/microsoft/generative-ai-with-javascript?WT.mc_id=academic-105485-koreyst)

---

### การเรียนรู้พื้นฐาน  
[![ML สำหรับผู้เริ่มต้น](https://img.shields.io/badge/ML%20for%20Beginners-22C55E?style=for-the-badge&labelColor=E5E7EB&color=22C55E)](https://aka.ms/ml-beginners?WT.mc_id=academic-105485-koreyst)  
[![Data Science สำหรับผู้เริ่มต้น](https://img.shields.io/badge/Data%20Science%20for%20Beginners-84CC16?style=for-the-badge&labelColor=E5E7EB&color=84CC16)](https://aka.ms/datascience-beginners?WT.mc_id=academic-105485-koreyst)  
[![AI สำหรับผู้เริ่มต้น](https://img.shields.io/badge/AI%20for%20Beginners-A3E635?style=for-the-badge&labelColor=E5E7EB&color=A3E635)](https://aka.ms/ai-beginners?WT.mc_id=academic-105485-koreyst)  
[![Cybersecurity สำหรับผู้เริ่มต้น](https://img.shields.io/badge/Cybersecurity%20for%20Beginners-F97316?style=for-the-badge&labelColor=E5E7EB&color=F97316)](https://github.com/microsoft/Security-101?WT.mc_id=academic-96948-sayoung)  
[![Web Dev สำหรับผู้เริ่มต้น](https://img.shields.io/badge/Web%20Dev%20for%20Beginners-EC4899?style=for-the-badge&labelColor=E5E7EB&color=EC4899)](https://aka.ms/webdev-beginners?WT.mc_id=academic-105485-koreyst)  
[![IoT สำหรับผู้เริ่มต้น](https://img.shields.io/badge/IoT%20for%20Beginners-14B8A6?style=for-the-badge&labelColor=E5E7EB&color=14B8A6)](https://aka.ms/iot-beginners?WT.mc_id=academic-105485-koreyst)  
[![XR Development สำหรับผู้เริ่มต้น](https://img.shields.io/badge/XR%20Development%20for%20Beginners-38BDF8?style=for-the-badge&labelColor=E5E7EB&color=38BDF8)](https://github.com/microsoft/xr-development-for-beginners?WT.mc_id=academic-105485-koreyst)

---

### ซีรีส์ Copilot  
[![Copilot สำหรับการเขียนโปรแกรมคู่ด้วย AI](https://img.shields.io/badge/Copilot%20for%20AI%20Paired%20Programming-FACC15?style=for-the-badge&labelColor=E5E7EB&color=FACC15)](https://aka.ms/GitHubCopilotAI?WT.mc_id=academic-105485-koreyst)  
[![Copilot สำหรับ C#/.NET](https://img.shields.io/badge/Copilot%20for%20C%23/.NET-FBBF24?style=for-the-badge&labelColor=E5E7EB&color=FBBF24)](https://github.com/microsoft/mastering-github-copilot-for-dotnet-csharp-developers?WT.mc_id=academic-105485-koreyst)  
[![Copilot Adventure](https://img.shields.io/badge/Copilot%20Adventure-FDE68A?style=for-the-badge&labelColor=E5E7EB&color=FDE68A)](https://github.com/microsoft/CopilotAdventures?WT.mc_id=academic-105485-koreyst)  
<!-- CO-OP TRANSLATOR OTHER COURSES END -->

## การขอความช่วยเหลือ  

**พบปัญหา?** ตรวจสอบ [คู่มือแก้ไขปัญหา](TROUBLESHOOTING.md) สำหรับวิธีแก้ไขปัญหาทั่วไป  

หากคุณติดขัดหรือมีคำถามเกี่ยวกับการสร้างแอป AI เข้าร่วม:  

[![Azure AI Foundry Discord](https://img.shields.io/badge/Discord-Azure_AI_Foundry_Community_Discord-blue?style=for-the-badge&logo=discord&color=5865f2&logoColor=fff)](https://aka.ms/foundry/discord)  

หากคุณมีข้อเสนอแนะเกี่ยวกับผลิตภัณฑ์หรือพบข้อผิดพลาดขณะสร้างแอป โปรดเยี่ยมชม:  

[![Azure AI Foundry Developer Forum](https://img.shields.io/badge/GitHub-Azure_AI_Foundry_Developer_Forum-blue?style=for-the-badge&logo=github&color=000000&logoColor=fff)](https://aka.ms/foundry/forum)  

---

**ข้อจำกัดความรับผิดชอบ**:  
เอกสารนี้ได้รับการแปลโดยใช้บริการแปลภาษา AI [Co-op Translator](https://github.com/Azure/co-op-translator) แม้ว่าเราจะพยายามให้การแปลมีความถูกต้อง แต่โปรดทราบว่าการแปลอัตโนมัติอาจมีข้อผิดพลาดหรือความไม่ถูกต้อง เอกสารต้นฉบับในภาษาดั้งเดิมควรถือเป็นแหล่งข้อมูลที่เชื่อถือได้ สำหรับข้อมูลสำคัญ ขอแนะนำให้ใช้บริการแปลภาษามืออาชีพ เราไม่รับผิดชอบต่อความเข้าใจผิดหรือการตีความผิดที่เกิดจากการใช้การแปลนี้