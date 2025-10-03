<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d24976d371de57bb657d3127f4195542",
  "translation_date": "2025-10-03T14:18:08+00:00",
  "source_file": "README.md",
  "language_code": "vi"
}
-->
# Khoa học Dữ liệu cho Người mới bắt đầu - Chương trình học

Azure Cloud Advocates tại Microsoft rất vui mừng giới thiệu chương trình học kéo dài 10 tuần, gồm 20 bài học về Khoa học Dữ liệu. Mỗi bài học bao gồm các bài kiểm tra trước và sau bài học, hướng dẫn viết để hoàn thành bài học, giải pháp và bài tập. Phương pháp học tập dựa trên dự án cho phép bạn học trong khi xây dựng, một cách hiệu quả để kỹ năng mới được ghi nhớ lâu dài.

**Cảm ơn chân thành đến các tác giả của chúng tôi:** [Jasmine Greenaway](https://www.twitter.com/paladique), [Dmitry Soshnikov](http://soshnikov.com), [Nitya Narasimhan](https://twitter.com/nitya), [Jalen McGee](https://twitter.com/JalenMcG), [Jen Looper](https://twitter.com/jenlooper), [Maud Levy](https://twitter.com/maudstweets), [Tiffany Souterre](https://twitter.com/TiffanySouterre), [Christopher Harrison](https://www.twitter.com/geektrainer).

**🙏 Đặc biệt cảm ơn 🙏 các [Microsoft Student Ambassador](https://studentambassadors.microsoft.com/) là tác giả, người đánh giá và đóng góp nội dung,** đặc biệt là Aaryan Arora, [Aditya Garg](https://github.com/AdityaGarg00), [Alondra Sanchez](https://www.linkedin.com/in/alondra-sanchez-molina/), [Ankita Singh](https://www.linkedin.com/in/ankitasingh007), [Anupam Mishra](https://www.linkedin.com/in/anupam--mishra/), [Arpita Das](https://www.linkedin.com/in/arpitadas01/), ChhailBihari Dubey, [Dibri Nsofor](https://www.linkedin.com/in/dibrinsofor), [Dishita Bhasin](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [Majd Safi](https://www.linkedin.com/in/majd-s/), [Max Blum](https://www.linkedin.com/in/max-blum-6036a1186/), [Miguel Correa](https://www.linkedin.com/in/miguelmque/), [Mohamma Iftekher (Iftu) Ebne Jalal](https://twitter.com/iftu119), [Nawrin Tabassum](https://www.linkedin.com/in/nawrin-tabassum), [Raymond Wangsa Putra](https://www.linkedin.com/in/raymond-wp/), [Rohit Yadav](https://www.linkedin.com/in/rty2423), Samridhi Sharma, [Sanya Sinha](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200),
[Sheena Narula](https://www.linkedin.com/in/sheena-narua-n/), [Tauqeer Ahmad](https://www.linkedin.com/in/tauqeerahmad5201/), Yogendrasingh Pawar , [Vidushi Gupta](https://www.linkedin.com/in/vidushi-gupta07/), [Jasleen Sondhi](https://www.linkedin.com/in/jasleen-sondhi/)

|![Sketchnote by @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.vi.png)|
|:---:|
| Khoa học Dữ liệu cho Người mới bắt đầu - _Sketchnote bởi [@nitya](https://twitter.com/nitya)_ |

### 🌐 Hỗ trợ đa ngôn ngữ

#### Được hỗ trợ qua GitHub Action (Tự động & Luôn cập nhật)

[French](../fr/README.md) | [Spanish](../es/README.md) | [German](../de/README.md) | [Russian](../ru/README.md) | [Arabic](../ar/README.md) | [Persian (Farsi)](../fa/README.md) | [Urdu](../ur/README.md) | [Chinese (Simplified)](../zh/README.md) | [Chinese (Traditional, Macau)](../mo/README.md) | [Chinese (Traditional, Hong Kong)](../hk/README.md) | [Chinese (Traditional, Taiwan)](../tw/README.md) | [Japanese](../ja/README.md) | [Korean](../ko/README.md) | [Hindi](../hi/README.md) | [Bengali](../bn/README.md) | [Marathi](../mr/README.md) | [Nepali](../ne/README.md) | [Punjabi (Gurmukhi)](../pa/README.md) | [Portuguese (Portugal)](../pt/README.md) | [Portuguese (Brazil)](../br/README.md) | [Italian](../it/README.md) | [Polish](../pl/README.md) | [Turkish](../tr/README.md) | [Greek](../el/README.md) | [Thai](../th/README.md) | [Swedish](../sv/README.md) | [Danish](../da/README.md) | [Norwegian](../no/README.md) | [Finnish](../fi/README.md) | [Dutch](../nl/README.md) | [Hebrew](../he/README.md) | [Vietnamese](./README.md) | [Indonesian](../id/README.md) | [Malay](../ms/README.md) | [Tagalog (Filipino)](../tl/README.md) | [Swahili](../sw/README.md) | [Hungarian](../hu/README.md) | [Czech](../cs/README.md) | [Slovak](../sk/README.md) | [Romanian](../ro/README.md) | [Bulgarian](../bg/README.md) | [Serbian (Cyrillic)](../sr/README.md) | [Croatian](../hr/README.md) | [Slovenian](../sl/README.md) | [Ukrainian](../uk/README.md) | [Burmese (Myanmar)](../my/README.md)

**Nếu bạn muốn có thêm các ngôn ngữ dịch, danh sách các ngôn ngữ được hỗ trợ có thể tìm thấy [tại đây](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md)**

#### Tham gia cộng đồng của chúng tôi 
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://aka.ms/ds4beginners/discord)

Chúng tôi có một chuỗi học tập với AI trên Discord đang diễn ra, tìm hiểu thêm và tham gia tại [Learn with AI Series](https://aka.ms/learnwithai/discord) từ ngày 18 - 30 tháng 9, 2025. Bạn sẽ nhận được mẹo và thủ thuật sử dụng GitHub Copilot cho Khoa học Dữ liệu.

![Learn with AI series](../../translated_images/1.2b28cdc6205e26fef6a21817fe5d83ae8b50fbd0a33e9fed0df05845da5b30b6.vi.jpg)

# Bạn là sinh viên?

Bắt đầu với các tài nguyên sau:

- [Trang Student Hub](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) Trong trang này, bạn sẽ tìm thấy các tài nguyên dành cho người mới bắt đầu, gói dành cho sinh viên và thậm chí là cách nhận voucher chứng chỉ miễn phí. Đây là một trang bạn nên đánh dấu và kiểm tra thường xuyên vì chúng tôi thay đổi nội dung ít nhất hàng tháng.
- [Microsoft Learn Student Ambassadors](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) Tham gia cộng đồng toàn cầu của các đại sứ sinh viên, đây có thể là cách bạn bước vào Microsoft.

# Bắt đầu

## 📚 Tài liệu

- **[Hướng dẫn cài đặt](INSTALLATION.md)** - Hướng dẫn từng bước để thiết lập cho người mới bắt đầu
- **[Hướng dẫn sử dụng](USAGE.md)** - Ví dụ và quy trình làm việc phổ biến
- **[Khắc phục sự cố](TROUBLESHOOTING.md)** - Giải pháp cho các vấn đề thường gặp
- **[Hướng dẫn đóng góp](CONTRIBUTING.md)** - Cách đóng góp cho dự án này
- **[Dành cho giáo viên](for-teachers.md)** - Hướng dẫn giảng dạy và tài nguyên lớp học

## 👨‍🎓 Dành cho sinh viên
> **Người mới hoàn toàn**: Mới với khoa học dữ liệu? Bắt đầu với [các ví dụ thân thiện với người mới bắt đầu](examples/README.md)! Những ví dụ đơn giản, được chú thích kỹ lưỡng này sẽ giúp bạn hiểu những điều cơ bản trước khi đi sâu vào toàn bộ chương trình học.
> **[Sinh viên](https://aka.ms/student-page)**: để sử dụng chương trình học này một cách độc lập, hãy fork toàn bộ repo và hoàn thành các bài tập theo cách của bạn, bắt đầu với bài kiểm tra trước bài học. Sau đó đọc bài giảng và hoàn thành các hoạt động còn lại. Hãy cố gắng tạo các dự án bằng cách hiểu bài học thay vì sao chép mã giải pháp; tuy nhiên, mã đó có sẵn trong các thư mục /solutions trong mỗi bài học dựa trên dự án. Một ý tưởng khác là tạo nhóm học tập với bạn bè và cùng nhau đi qua nội dung. Để học thêm, chúng tôi khuyến nghị [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum).

**Bắt đầu nhanh:**
1. Kiểm tra [Hướng dẫn cài đặt](INSTALLATION.md) để thiết lập môi trường của bạn
2. Xem lại [Hướng dẫn sử dụng](USAGE.md) để học cách làm việc với chương trình học
3. Bắt đầu với Bài học 1 và làm việc theo thứ tự
4. Tham gia cộng đồng [Discord của chúng tôi](https://aka.ms/ds4beginners/discord) để được hỗ trợ

## 👩‍🏫 Dành cho giáo viên

> **Giáo viên**: chúng tôi đã [bao gồm một số gợi ý](for-teachers.md) về cách sử dụng chương trình học này. Chúng tôi rất mong nhận được phản hồi của bạn [trong diễn đàn thảo luận của chúng tôi](https://github.com/microsoft/Data-Science-For-Beginners/discussions)!

## Gặp gỡ đội ngũ

[![Video giới thiệu](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "Video giới thiệu")

**Gif bởi** [Mohit Jaisal](https://www.linkedin.com/in/mohitjaisal)

> 🎥 Nhấp vào hình ảnh trên để xem video về dự án và những người đã tạo ra nó!

## Phương pháp giảng dạy

Chúng tôi đã chọn hai nguyên tắc giảng dạy khi xây dựng chương trình học này: đảm bảo rằng nó dựa trên dự án và bao gồm các bài kiểm tra thường xuyên. Đến cuối chuỗi này, sinh viên sẽ học được các nguyên tắc cơ bản của khoa học dữ liệu, bao gồm các khái niệm đạo đức, chuẩn bị dữ liệu, các cách làm việc khác nhau với dữ liệu, trực quan hóa dữ liệu, phân tích dữ liệu, các trường hợp sử dụng thực tế của khoa học dữ liệu và nhiều hơn nữa.
Ngoài ra, một bài kiểm tra nhỏ trước lớp giúp học sinh định hướng mục tiêu học tập về một chủ đề, trong khi bài kiểm tra thứ hai sau lớp đảm bảo việc ghi nhớ lâu hơn. Chương trình học này được thiết kế linh hoạt và thú vị, có thể học toàn bộ hoặc từng phần. Các dự án bắt đầu từ quy mô nhỏ và trở nên phức tạp hơn vào cuối chu kỳ 10 tuần.

> Tìm hiểu [Quy tắc ứng xử](CODE_OF_CONDUCT.md), [Hướng dẫn đóng góp](CONTRIBUTING.md), [Hướng dẫn dịch thuật](TRANSLATIONS.md). Chúng tôi hoan nghênh những phản hồi mang tính xây dựng của bạn!

## Mỗi bài học bao gồm:

- Ghi chú hình ảnh (tùy chọn)
- Video bổ sung (tùy chọn)
- Bài kiểm tra khởi động trước bài học
- Bài học viết
- Đối với các bài học dựa trên dự án, hướng dẫn từng bước để xây dựng dự án
- Kiểm tra kiến thức
- Một thử thách
- Tài liệu đọc bổ sung
- Bài tập
- [Bài kiểm tra sau bài học](https://ff-quizzes.netlify.app/en/)

> **Lưu ý về bài kiểm tra**: Tất cả các bài kiểm tra nằm trong thư mục Quiz-App, với tổng cộng 40 bài kiểm tra, mỗi bài gồm ba câu hỏi. Các bài kiểm tra được liên kết từ trong bài học, nhưng ứng dụng kiểm tra có thể chạy cục bộ hoặc triển khai trên Azure; hãy làm theo hướng dẫn trong thư mục `quiz-app`. Các bài kiểm tra đang dần được bản địa hóa.

## 🎓 Ví dụ thân thiện với người mới bắt đầu

**Mới làm quen với Khoa học Dữ liệu?** Chúng tôi đã tạo một [thư mục ví dụ](examples/README.md) đặc biệt với mã đơn giản, được chú thích rõ ràng để giúp bạn bắt đầu:

- 🌟 **Hello World** - Chương trình khoa học dữ liệu đầu tiên của bạn
- 📂 **Tải dữ liệu** - Học cách đọc và khám phá các tập dữ liệu
- 📊 **Phân tích đơn giản** - Tính toán thống kê và tìm kiếm mẫu
- 📈 **Trực quan hóa cơ bản** - Tạo biểu đồ và đồ thị
- 🔬 **Dự án thực tế** - Quy trình làm việc hoàn chỉnh từ đầu đến cuối

Mỗi ví dụ đều có chú thích chi tiết giải thích từng bước, rất phù hợp cho người mới bắt đầu!

👉 **[Bắt đầu với các ví dụ](examples/README.md)** 👈

## Các bài học


|![ Ghi chú hình ảnh của @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.vi.png)|
|:---:|
| Khoa học Dữ liệu cho Người mới bắt đầu: Lộ trình - _Ghi chú hình ảnh của [@nitya](https://twitter.com/nitya)_ |


| Số bài học | Chủ đề | Nhóm bài học | Mục tiêu học tập | Liên kết bài học | Tác giả |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | Định nghĩa Khoa học Dữ liệu | [Giới thiệu](1-Introduction/README.md) | Tìm hiểu các khái niệm cơ bản về khoa học dữ liệu và cách nó liên quan đến trí tuệ nhân tạo, học máy và dữ liệu lớn. | [bài học](1-Introduction/01-defining-data-science/README.md) [video](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | Đạo đức Khoa học Dữ liệu | [Giới thiệu](1-Introduction/README.md) | Các khái niệm, thách thức và khung đạo đức dữ liệu. | [bài học](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | Định nghĩa Dữ liệu | [Giới thiệu](1-Introduction/README.md) | Cách phân loại dữ liệu và các nguồn phổ biến của nó. | [bài học](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | Giới thiệu về Thống kê & Xác suất | [Giới thiệu](1-Introduction/README.md) | Các kỹ thuật toán học về xác suất và thống kê để hiểu dữ liệu. | [bài học](1-Introduction/04-stats-and-probability/README.md) [video](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | Làm việc với Dữ liệu Quan hệ | [Làm việc với Dữ liệu](2-Working-With-Data/README.md) | Giới thiệu về dữ liệu quan hệ và các nguyên tắc cơ bản để khám phá và phân tích dữ liệu quan hệ bằng Ngôn ngữ Truy vấn Có cấu trúc, còn được gọi là SQL (phát âm là “see-quell”). | [bài học](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | Làm việc với Dữ liệu NoSQL | [Làm việc với Dữ liệu](2-Working-With-Data/README.md) | Giới thiệu về dữ liệu phi quan hệ, các loại khác nhau của nó và các nguyên tắc cơ bản để khám phá và phân tích cơ sở dữ liệu tài liệu. | [bài học](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | Làm việc với Python | [Làm việc với Dữ liệu](2-Working-With-Data/README.md) | Các nguyên tắc cơ bản về sử dụng Python để khám phá dữ liệu với các thư viện như Pandas. Hiểu biết cơ bản về lập trình Python được khuyến nghị. | [bài học](2-Working-With-Data/07-python/README.md) [video](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | Chuẩn bị Dữ liệu | [Làm việc với Dữ liệu](2-Working-With-Data/README.md) | Các chủ đề về kỹ thuật dữ liệu để làm sạch và chuyển đổi dữ liệu nhằm xử lý các thách thức về dữ liệu thiếu, không chính xác hoặc không đầy đủ. | [bài học](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | Trực quan hóa Số lượng | [Trực quan hóa Dữ liệu](3-Data-Visualization/README.md) | Tìm hiểu cách sử dụng Matplotlib để trực quan hóa dữ liệu chim 🦆 | [bài học](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | Trực quan hóa Phân phối Dữ liệu | [Trực quan hóa Dữ liệu](3-Data-Visualization/README.md) | Trực quan hóa các quan sát và xu hướng trong một khoảng thời gian. | [bài học](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | Trực quan hóa Tỷ lệ | [Trực quan hóa Dữ liệu](3-Data-Visualization/README.md) | Trực quan hóa các phần trăm rời rạc và nhóm. | [bài học](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | Trực quan hóa Mối quan hệ | [Trực quan hóa Dữ liệu](3-Data-Visualization/README.md) | Trực quan hóa các kết nối và mối tương quan giữa các tập dữ liệu và các biến của chúng. | [bài học](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | Trực quan hóa Có ý nghĩa | [Trực quan hóa Dữ liệu](3-Data-Visualization/README.md) | Các kỹ thuật và hướng dẫn để làm cho các trực quan hóa của bạn có giá trị trong việc giải quyết vấn đề hiệu quả và cung cấp thông tin chi tiết. | [bài học](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | Giới thiệu về vòng đời Khoa học Dữ liệu | [Vòng đời](4-Data-Science-Lifecycle/README.md) | Giới thiệu về vòng đời khoa học dữ liệu và bước đầu tiên của nó là thu thập và trích xuất dữ liệu. | [bài học](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | Phân tích | [Vòng đời](4-Data-Science-Lifecycle/README.md) | Giai đoạn này của vòng đời khoa học dữ liệu tập trung vào các kỹ thuật phân tích dữ liệu. | [bài học](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | Giao tiếp | [Vòng đời](4-Data-Science-Lifecycle/README.md) | Giai đoạn này của vòng đời khoa học dữ liệu tập trung vào việc trình bày các thông tin chi tiết từ dữ liệu theo cách giúp người ra quyết định dễ dàng hiểu hơn. | [bài học](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | Khoa học Dữ liệu trên Đám mây | [Dữ liệu Đám mây](5-Data-Science-In-Cloud/README.md) | Loạt bài học này giới thiệu khoa học dữ liệu trên đám mây và các lợi ích của nó. | [bài học](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) và [Maud](https://twitter.com/maudstweets) |
| 18 | Khoa học Dữ liệu trên Đám mây | [Dữ liệu Đám mây](5-Data-Science-In-Cloud/README.md) | Huấn luyện mô hình bằng các công cụ Low Code. |[bài học](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) và [Maud](https://twitter.com/maudstweets) |
| 19 | Khoa học Dữ liệu trên Đám mây | [Dữ liệu Đám mây](5-Data-Science-In-Cloud/README.md) | Triển khai mô hình với Azure Machine Learning Studio. | [bài học](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) và [Maud](https://twitter.com/maudstweets) |
| 20 | Khoa học Dữ liệu trong Thực tế | [Trong Thực tế](6-Data-Science-In-Wild/README.md) | Các dự án khoa học dữ liệu trong thế giới thực. | [bài học](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

Làm theo các bước sau để mở mẫu này trong Codespace:
1. Nhấp vào menu thả xuống Code và chọn tùy chọn Open with Codespaces.
2. Chọn + New codespace ở dưới cùng của bảng.
Để biết thêm thông tin, hãy xem [tài liệu GitHub](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace).

## VSCode Remote - Containers
Làm theo các bước sau để mở kho lưu trữ này trong một container bằng máy tính cục bộ của bạn và VSCode sử dụng tiện ích mở rộng VS Code Remote - Containers:

1. Nếu đây là lần đầu tiên bạn sử dụng container phát triển, hãy đảm bảo hệ thống của bạn đáp ứng các yêu cầu (ví dụ: đã cài đặt Docker) trong [tài liệu bắt đầu](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started).

Để sử dụng kho lưu trữ này, bạn có thể mở kho lưu trữ trong một volume Docker cách ly:

**Lưu ý**: Phía sau, điều này sẽ sử dụng lệnh Remote-Containers: **Clone Repository in Container Volume...** để sao chép mã nguồn trong một volume Docker thay vì hệ thống tệp cục bộ. [Volumes](https://docs.docker.com/storage/volumes/) là cơ chế ưu tiên để lưu trữ dữ liệu container.

Hoặc mở một phiên bản đã sao chép hoặc tải xuống cục bộ của kho lưu trữ:

- Sao chép kho lưu trữ này vào hệ thống tệp cục bộ của bạn.
- Nhấn F1 và chọn lệnh **Remote-Containers: Open Folder in Container...**.
- Chọn bản sao đã sao chép của thư mục này, chờ container khởi động và thử nghiệm.

## Truy cập ngoại tuyến

Bạn có thể chạy tài liệu này ngoại tuyến bằng cách sử dụng [Docsify](https://docsify.js.org/#/). Fork kho lưu trữ này, [cài đặt Docsify](https://docsify.js.org/#/quickstart) trên máy tính cục bộ của bạn, sau đó trong thư mục gốc của kho lưu trữ này, gõ `docsify serve`. Trang web sẽ được phục vụ trên cổng 3000 trên localhost của bạn: `localhost:3000`.

> Lưu ý, các notebook sẽ không được hiển thị qua Docsify, vì vậy khi bạn cần chạy một notebook, hãy làm điều đó riêng biệt trong VS Code chạy kernel Python.

## Các chương trình học khác

Nhóm của chúng tôi sản xuất các chương trình học khác! Hãy xem:

- [Edge AI cho Người mới bắt đầu](https://aka.ms/edgeai-for-beginners)
- [AI Agents cho Người mới bắt đầu](https://aka.ms/ai-agents-beginners)
- [Generative AI cho Người mới bắt đầu](https://aka.ms/genai-beginners)
- [Generative AI cho Người mới bắt đầu .NET](https://github.com/microsoft/Generative-AI-for-beginners-dotnet)
- [Generative AI với JavaScript](https://github.com/microsoft/generative-ai-with-javascript)
- [Generative AI với Java](https://aka.ms/genaijava)
- [AI cho Người mới bắt đầu](https://aka.ms/ai-beginners)
- [Khoa học Dữ liệu cho Người mới bắt đầu](https://aka.ms/datascience-beginners)
- [Bash cho Người mới bắt đầu](https://github.com/microsoft/bash-for-beginners)
- [ML cho Người mới bắt đầu](https://aka.ms/ml-beginners)
- [An ninh mạng cho Người mới bắt đầu](https://github.com/microsoft/Security-101) 
- [Phát triển Web cho Người mới bắt đầu](https://aka.ms/webdev-beginners)
- [IoT cho Người mới bắt đầu](https://aka.ms/iot-beginners)
- [Học máy cho Người mới bắt đầu](https://aka.ms/ml-beginners)
- [Phát triển XR cho Người mới bắt đầu](https://aka.ms/xr-dev-for-beginners)
- [Làm chủ GitHub Copilot cho Lập trình Đôi với AI](https://aka.ms/GitHubCopilotAI)
- [Phát triển XR cho Người mới bắt đầu](https://github.com/microsoft/xr-development-for-beginners)
- [Làm chủ GitHub Copilot cho Nhà phát triển C#/.NET](https://github.com/microsoft/mastering-github-copilot-for-dotnet-csharp-developers)
- [Chọn Cuộc Phiêu Lưu Copilot của Bạn](https://github.com/microsoft/CopilotAdventures)

## Nhận Hỗ Trợ

**Gặp vấn đề?** Xem [Hướng dẫn Khắc phục sự cố](TROUBLESHOOTING.md) để tìm giải pháp cho các vấn đề thường gặp.

Nếu bạn gặp khó khăn hoặc có câu hỏi về việc xây dựng ứng dụng AI, hãy tham gia:

[![Azure AI Foundry Discord](https://img.shields.io/badge/Discord-Azure_AI_Foundry_Community_Discord-blue?style=for-the-badge&logo=discord&color=5865f2&logoColor=fff)](https://aka.ms/foundry/discord)

Nếu bạn có phản hồi về sản phẩm hoặc gặp lỗi trong quá trình xây dựng, hãy truy cập:

[![Azure AI Foundry Developer Forum](https://img.shields.io/badge/GitHub-Azure_AI_Foundry_Developer_Forum-blue?style=for-the-badge&logo=github&color=000000&logoColor=fff)](https://aka.ms/foundry/forum)

---

**Tuyên bố miễn trừ trách nhiệm**:  
Tài liệu này đã được dịch bằng dịch vụ dịch thuật AI [Co-op Translator](https://github.com/Azure/co-op-translator). Mặc dù chúng tôi cố gắng đảm bảo độ chính xác, xin lưu ý rằng các bản dịch tự động có thể chứa lỗi hoặc không chính xác. Tài liệu gốc bằng ngôn ngữ bản địa nên được coi là nguồn thông tin chính thức. Đối với các thông tin quan trọng, khuyến nghị sử dụng dịch vụ dịch thuật chuyên nghiệp bởi con người. Chúng tôi không chịu trách nhiệm cho bất kỳ sự hiểu lầm hoặc diễn giải sai nào phát sinh từ việc sử dụng bản dịch này.