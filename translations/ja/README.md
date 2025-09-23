<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "ae529efe508173a92d4019d86744ec00",
  "translation_date": "2025-09-23T08:53:54+00:00",
  "source_file": "README.md",
  "language_code": "ja"
}
-->
# 初心者のためのデータサイエンス - カリキュラム

Azure Cloud Advocates at Microsoftは、データサイエンスに関する10週間、20レッスンのカリキュラムを提供します。各レッスンには、事前・事後のクイズ、レッスンを完了するための手順書、解答例、課題が含まれています。このプロジェクトベースの教育法により、学びながら構築することで、新しいスキルを効果的に身につけることができます。

**著者の皆さんに感謝します:** [Jasmine Greenaway](https://www.twitter.com/paladique), [Dmitry Soshnikov](http://soshnikov.com), [Nitya Narasimhan](https://twitter.com/nitya), [Jalen McGee](https://twitter.com/JalenMcG), [Jen Looper](https://twitter.com/jenlooper), [Maud Levy](https://twitter.com/maudstweets), [Tiffany Souterre](https://twitter.com/TiffanySouterre), [Christopher Harrison](https://www.twitter.com/geektrainer).

**🙏 特別な感謝 🙏 を以下の[Microsoft Student Ambassador](https://studentambassadors.microsoft.com/)の著者、レビュアー、コンテンツ貢献者の皆さんに:** 特にAaryan Arora, [Aditya Garg](https://github.com/AdityaGarg00), [Alondra Sanchez](https://www.linkedin.com/in/alondra-sanchez-molina/), [Ankita Singh](https://www.linkedin.com/in/ankitasingh007), [Anupam Mishra](https://www.linkedin.com/in/anupam--mishra/), [Arpita Das](https://www.linkedin.com/in/arpitadas01/), ChhailBihari Dubey, [Dibri Nsofor](https://www.linkedin.com/in/dibrinsofor), [Dishita Bhasin](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [Majd Safi](https://www.linkedin.com/in/majd-s/), [Max Blum](https://www.linkedin.com/in/max-blum-6036a1186/), [Miguel Correa](https://www.linkedin.com/in/miguelmque/), [Mohamma Iftekher (Iftu) Ebne Jalal](https://twitter.com/iftu119), [Nawrin Tabassum](https://www.linkedin.com/in/nawrin-tabassum), [Raymond Wangsa Putra](https://www.linkedin.com/in/raymond-wp/), [Rohit Yadav](https://www.linkedin.com/in/rty2423), Samridhi Sharma, [Sanya Sinha](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200), [Sheena Narula](https://www.linkedin.com/in/sheena-narua-n/), [Tauqeer Ahmad](https://www.linkedin.com/in/tauqeerahmad5201/), Yogendrasingh Pawar, [Vidushi Gupta](https://www.linkedin.com/in/vidushi-gupta07/), [Jasleen Sondhi](https://www.linkedin.com/in/jasleen-sondhi/)

|![@sketchthedocsによるスケッチノート https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.ja.png)|
|:---:|
| 初心者のためのデータサイエンス - _[@nitya](https://twitter.com/nitya)によるスケッチノート_ |

### 🌐 多言語サポート

#### GitHub Actionを通じてサポート（自動化＆常に最新）

[フランス語](../fr/README.md) | [スペイン語](../es/README.md) | [ドイツ語](../de/README.md) | [ロシア語](../ru/README.md) | [アラビア語](../ar/README.md) | [ペルシャ語 (ファルシ)](../fa/README.md) | [ウルドゥー語](../ur/README.md) | [中国語 (簡体字)](../zh/README.md) | [中国語 (繁体字, マカオ)](../mo/README.md) | [中国語 (繁体字, 香港)](../hk/README.md) | [中国語 (繁体字, 台湾)](../tw/README.md) | [日本語](./README.md) | [韓国語](../ko/README.md) | [ヒンディー語](../hi/README.md) | [ベンガル語](../bn/README.md) | [マラーティー語](../mr/README.md) | [ネパール語](../ne/README.md) | [パンジャブ語 (グルムキー)](../pa/README.md) | [ポルトガル語 (ポルトガル)](../pt/README.md) | [ポルトガル語 (ブラジル)](../br/README.md) | [イタリア語](../it/README.md) | [ポーランド語](../pl/README.md) | [トルコ語](../tr/README.md) | [ギリシャ語](../el/README.md) | [タイ語](../th/README.md) | [スウェーデン語](../sv/README.md) | [デンマーク語](../da/README.md) | [ノルウェー語](../no/README.md) | [フィンランド語](../fi/README.md) | [オランダ語](../nl/README.md) | [ヘブライ語](../he/README.md) | [ベトナム語](../vi/README.md) | [インドネシア語](../id/README.md) | [マレー語](../ms/README.md) | [タガログ語 (フィリピン)](../tl/README.md) | [スワヒリ語](../sw/README.md) | [ハンガリー語](../hu/README.md) | [チェコ語](../cs/README.md) | [スロバキア語](../sk/README.md) | [ルーマニア語](../ro/README.md) | [ブルガリア語](../bg/README.md) | [セルビア語 (キリル文字)](../sr/README.md) | [クロアチア語](../hr/README.md) | [スロベニア語](../sl/README.md) | [ウクライナ語](../uk/README.md) | [ビルマ語 (ミャンマー)](../my/README.md)

**追加の翻訳を希望する場合は、[こちら](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md)にサポートされている言語が記載されています。**

#### コミュニティに参加しよう
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://aka.ms/ds4beginners/discord)

現在、AIを使った学習シリーズをDiscordで開催中です。詳細を確認し、[Learn with AI Series](https://aka.ms/learnwithai/discord)に2025年9月18日から30日まで参加してください。GitHub Copilotをデータサイエンスで活用するためのヒントやコツを学べます。

![Learn with AI series](../../translated_images/1.2b28cdc6205e26fef6a21817fe5d83ae8b50fbd0a33e9fed0df05845da5b30b6.ja.jpg)

# 学生の皆さんへ

以下のリソースから始めてみましょう：

- [Student Hubページ](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) このページでは、初心者向けリソース、学生向けパック、さらには無料の認定バウチャーを取得する方法が見つかります。このページはブックマークして、定期的にチェックすることをお勧めします。少なくとも月に一度はコンテンツが更新されます。
- [Microsoft Learn Student Ambassadors](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) グローバルな学生アンバサダーコミュニティに参加しましょう。これがMicrosoftへの道になるかもしれません。

# 始めに

> **教師の皆さん**: このカリキュラムの使用方法について[いくつかの提案](for-teachers.md)を含めています。フィードバックは[ディスカッションフォーラム](https://github.com/microsoft/Data-Science-For-Beginners/discussions)でお待ちしています！

> **[学生の皆さん](https://aka.ms/student-page)**: このカリキュラムを自分で使用するには、リポジトリ全体をフォークし、事前クイズから始めて自分で演習を完了してください。その後、講義を読み、残りの活動を完了します。解答コードをコピーするのではなく、レッスンを理解しながらプロジェクトを作成することをお勧めします。ただし、解答コードは各プロジェクト指向のレッスンの/solutionsフォルダーにあります。また、友達と一緒に勉強グループを作り、コンテンツを一緒に進めるのも良いアイデアです。さらに学びたい場合は、[Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum)をお勧めします。

## チーム紹介

[![プロモーションビデオ](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "プロモーションビデオ")

**Gif作成者:** [Mohit Jaisal](https://www.linkedin.com/in/mohitjaisal)

> 🎥 上の画像をクリックすると、このプロジェクトと作成者についてのビデオが見られます！

## 教育方針

このカリキュラムを構築する際、プロジェクトベースであることと頻繁なクイズを含むことの2つの教育方針を採用しました。このシリーズの終わりまでに、学生はデータサイエンスの基本原則（倫理的概念、データ準備、データの操作方法、データ可視化、データ分析、データサイエンスの実世界での使用例など）を学びます。

さらに、授業前の低リスクなクイズは、学生がトピックを学ぶ意図を設定し、授業後のクイズはさらなる記憶定着を促します。このカリキュラムは柔軟で楽しいものとして設計されており、全体または一部を受講することができます。プロジェクトは小さなものから始まり、10週間のサイクルの終わりには徐々に複雑になります。

> [行動規範](CODE_OF_CONDUCT.md)、[貢献ガイドライン](CONTRIBUTING.md)、[翻訳ガイドライン](TRANSLATIONS.md)をご覧ください。建設的なフィードバックをお待ちしています！

## 各レッスンには以下が含まれます：

- オプションのスケッチノート
- オプションの補足ビデオ
- レッスン前のウォームアップクイズ
- 書面によるレッスン
- プロジェクトベースのレッスンの場合、プロジェクトの構築方法に関するステップバイステップガイド
- 知識チェック
- チャレンジ
- 補足読書
- 課題
- [レッスン後のクイズ](https://ff-quizzes.netlify.app/en/)

> **クイズについての注意**: すべてのクイズはQuiz-Appフォルダーに含まれており、合計40のクイズが各3問ずつあります。レッスン内からリンクされていますが、クイズアプリはローカルで実行するか、Azureにデプロイすることができます。`quiz-app`フォルダーの指示に従ってください。クイズは徐々にローカライズされています。

## レッスン
|![ Sketchnote by @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.ja.png)|
|:---:|
| データサイエンス初心者向けロードマップ - _スケッチノート作成者: [@nitya](https://twitter.com/nitya)_ |

| レッスン番号 | トピック | レッスングループ | 学習目標 | リンクされたレッスン | 著者 |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | データサイエンスの定義 | [イントロダクション](1-Introduction/README.md) | データサイエンスの基本概念と、それが人工知能、機械学習、大規模データとどのように関連しているかを学ぶ。 | [レッスン](1-Introduction/01-defining-data-science/README.md) [動画](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | データサイエンス倫理 | [イントロダクション](1-Introduction/README.md) | データ倫理の概念、課題、フレームワーク。 | [レッスン](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | データの定義 | [イントロダクション](1-Introduction/README.md) | データの分類方法とその一般的なソース。 | [レッスン](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | 統計と確率のイントロダクション | [イントロダクション](1-Introduction/README.md) | データを理解するための確率と統計の数学的手法。 | [レッスン](1-Introduction/04-stats-and-probability/README.md) [動画](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | リレーショナルデータの操作 | [データ操作](2-Working-With-Data/README.md) | リレーショナルデータの紹介と、SQL（「シークエル」と発音）を使用したリレーショナルデータの探索と分析の基本。 | [レッスン](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | NoSQLデータの操作 | [データ操作](2-Working-With-Data/README.md) | 非リレーショナルデータの紹介、そのさまざまな種類、およびドキュメントデータベースの探索と分析の基本。 | [レッスン](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | Pythonの操作 | [データ操作](2-Working-With-Data/README.md) | Pandasなどのライブラリを使用したデータ探索のためのPythonの基本。Pythonプログラミングの基礎的な理解が推奨される。 | [レッスン](2-Working-With-Data/07-python/README.md) [動画](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | データ準備 | [データ操作](2-Working-With-Data/README.md) | 欠損、不正確、不完全なデータの課題に対処するためのデータクリーニングと変換技術に関するトピック。 | [レッスン](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | 数量の可視化 | [データ可視化](3-Data-Visualization/README.md) | Matplotlibを使用して鳥のデータを可視化する方法を学ぶ 🦆 | [レッスン](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | データ分布の可視化 | [データ可視化](3-Data-Visualization/README.md) | 区間内の観察と傾向を可視化する。 | [レッスン](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | 比率の可視化 | [データ可視化](3-Data-Visualization/README.md) | 離散的およびグループ化された割合を可視化する。 | [レッスン](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | 関係性の可視化 | [データ可視化](3-Data-Visualization/README.md) | データセットとその変数間の接続と相関を可視化する。 | [レッスン](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | 意味のある可視化 | [データ可視化](3-Data-Visualization/README.md) | 問題解決と洞察を効果的にするための可視化を価値あるものにする技術とガイダンス。 | [レッスン](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | データサイエンスライフサイクルのイントロダクション | [ライフサイクル](4-Data-Science-Lifecycle/README.md) | データサイエンスライフサイクルの紹介と、データの取得と抽出の最初のステップ。 | [レッスン](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | 分析 | [ライフサイクル](4-Data-Science-Lifecycle/README.md) | データサイエンスライフサイクルのこのフェーズでは、データを分析する技術に焦点を当てる。 | [レッスン](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | コミュニケーション | [ライフサイクル](4-Data-Science-Lifecycle/README.md) | データサイエンスライフサイクルのこのフェーズでは、意思決定者が理解しやすい形でデータから得られた洞察を提示することに焦点を当てる。 | [レッスン](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | クラウドでのデータサイエンス | [クラウドデータ](5-Data-Science-In-Cloud/README.md) | クラウドでのデータサイエンスとその利点を紹介する一連のレッスン。 | [レッスン](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) と [Maud](https://twitter.com/maudstweets) |
| 18 | クラウドでのデータサイエンス | [クラウドデータ](5-Data-Science-In-Cloud/README.md) | ローコードツールを使用したモデルのトレーニング。 |[レッスン](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) と [Maud](https://twitter.com/maudstweets) |
| 19 | クラウドでのデータサイエンス | [クラウドデータ](5-Data-Science-In-Cloud/README.md) | Azure Machine Learning Studioを使用したモデルのデプロイ。 | [レッスン](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) と [Maud](https://twitter.com/maudstweets) |
| 20 | 実世界でのデータサイエンス | [実世界](6-Data-Science-In-Wild/README.md) | 実世界でのデータサイエンス駆動型プロジェクト。 | [レッスン](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

Codespaceでこのサンプルを開く手順:
1. Codeドロップダウンメニューをクリックし、「Open with Codespaces」オプションを選択。
2. ペインの下部で「+ New codespace」を選択。
詳細については、[GitHubのドキュメント](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace)を参照してください。

## VSCode Remote - Containers
VSCodeのRemote - Containers拡張機能を使用して、ローカルマシンでこのリポジトリをコンテナ内で開く手順:

1. 初めて開発コンテナを使用する場合は、[開始ガイド](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started)でシステムが必要条件を満たしていることを確認してください（例: Dockerがインストールされていること）。

このリポジトリを使用するには、以下のいずれかの方法を選択してください:

**注意**: 内部的には、Remote-Containers: **Clone Repository in Container Volume...** コマンドを使用して、ソースコードをローカルファイルシステムではなくDockerボリュームにクローンします。[ボリューム](https://docs.docker.com/storage/volumes/)はコンテナデータを永続化するための推奨メカニズムです。

または、ローカルにクローンまたはダウンロードしたリポジトリを開く:

- このリポジトリをローカルファイルシステムにクローン。
- F1キーを押して、**Remote-Containers: Open Folder in Container...** コマンドを選択。
- クローンしたフォルダを選択し、コンテナが起動するのを待って試してみてください。

## オフラインアクセス

[Docsify](https://docsify.js.org/#/)を使用して、このドキュメントをオフラインで実行できます。このリポジトリをフォークし、ローカルマシンに[Docsifyをインストール](https://docsify.js.org/#/quickstart)した後、このリポジトリのルートフォルダで`docsify serve`と入力してください。ウェブサイトはローカルホストのポート3000で提供されます: `localhost:3000`。

> 注意: Docsifyではノートブックはレンダリングされません。そのため、ノートブックを実行する必要がある場合は、Pythonカーネルを使用してVS Codeで別途実行してください。

## その他のカリキュラム

私たちのチームは他のカリキュラムも提供しています！以下をチェックしてください:

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

