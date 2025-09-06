<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "7332da4946897c5885e9ca5bc24de96b",
  "translation_date": "2025-09-06T10:48:39+00:00",
  "source_file": "README.md",
  "language_code": "pa"
}
-->
# ਡਾਟਾ ਸਾਇੰਸ ਸ਼ੁਰੂਆਤੀ ਲਈ - ਇੱਕ ਪਾਠਕ੍ਰਮ

Azure Cloud Advocates ਮਾਈਕਰੋਸਾਫਟ ਵਿੱਚ 10 ਹਫ਼ਤਿਆਂ ਦਾ, 20 ਪਾਠਾਂ ਦਾ ਪਾਠਕ੍ਰਮ ਪੇਸ਼ ਕਰਨ ਵਿੱਚ ਖੁਸ਼ ਹਨ ਜੋ ਡਾਟਾ ਸਾਇੰਸ ਬਾਰੇ ਹੈ। ਹਰ ਪਾਠ ਵਿੱਚ ਪਾਠ ਤੋਂ ਪਹਿਲਾਂ ਅਤੇ ਪਾਠ ਤੋਂ ਬਾਅਦ ਦੇ ਪ੍ਰਸ਼ਨ, ਪਾਠ ਪੂਰਾ ਕਰਨ ਲਈ ਲਿਖਤ ਨਿਰਦੇਸ਼, ਇੱਕ ਹੱਲ ਅਤੇ ਇੱਕ ਅਸਾਈਨਮੈਂਟ ਸ਼ਾਮਲ ਹੈ। ਸਾਡੇ ਪ੍ਰੋਜੈਕਟ-ਅਧਾਰਤ ਪੈਡਾਗੌਜੀ ਤੁਹਾਨੂੰ ਸਿਖਾਉਣ ਦੇ ਦੌਰਾਨ ਬਣਾਉਣ ਦੀ ਆਗਿਆ ਦਿੰਦਾ ਹੈ, ਜੋ ਨਵੀਆਂ ਹੁਨਰਾਂ ਨੂੰ 'ਟਿਕਾਉਣ' ਦਾ ਸਾਬਤ ਤਰੀਕਾ ਹੈ।

**ਸਾਡੇ ਲੇਖਕਾਂ ਨੂੰ ਦਿਲੋਂ ਧੰਨਵਾਦ:** [Jasmine Greenaway](https://www.twitter.com/paladique), [Dmitry Soshnikov](http://soshnikov.com), [Nitya Narasimhan](https://twitter.com/nitya), [Jalen McGee](https://twitter.com/JalenMcG), [Jen Looper](https://twitter.com/jenlooper), [Maud Levy](https://twitter.com/maudstweets), [Tiffany Souterre](https://twitter.com/TiffanySouterre), [Christopher Harrison](https://www.twitter.com/geektrainer)।

**🙏 ਵਿਸ਼ੇਸ਼ ਧੰਨਵਾਦ 🙏 ਸਾਡੇ [Microsoft Student Ambassador](https://studentambassadors.microsoft.com/) ਲੇਖਕਾਂ, ਸਮੀਖਾਕਾਰਾਂ ਅਤੇ ਸਮੱਗਰੀ ਯੋਗਦਾਨਕਰਤਾਵਾਂ ਨੂੰ,** ਖਾਸ ਤੌਰ 'ਤੇ Aaryan Arora, [Aditya Garg](https://github.com/AdityaGarg00), [Alondra Sanchez](https://www.linkedin.com/in/alondra-sanchez-molina/), [Ankita Singh](https://www.linkedin.com/in/ankitasingh007), [Anupam Mishra](https://www.linkedin.com/in/anupam--mishra/), [Arpita Das](https://www.linkedin.com/in/arpitadas01/), ChhailBihari Dubey, [Dibri Nsofor](https://www.linkedin.com/in/dibrinsofor), [Dishita Bhasin](https://www.linkedin.com/in/dishita-bhasin-7065281bb), [Majd Safi](https://www.linkedin.com/in/majd-s/), [Max Blum](https://www.linkedin.com/in/max-blum-6036a1186/), [Miguel Correa](https://www.linkedin.com/in/miguelmque/), [Mohamma Iftekher (Iftu) Ebne Jalal](https://twitter.com/iftu119), [Nawrin Tabassum](https://www.linkedin.com/in/nawrin-tabassum), [Raymond Wangsa Putra](https://www.linkedin.com/in/raymond-wp/), [Rohit Yadav](https://www.linkedin.com/in/rty2423), Samridhi Sharma, [Sanya Sinha](https://www.linkedin.com/mwlite/in/sanya-sinha-13aab1200), [Sheena Narula](https://www.linkedin.com/in/sheena-narua-n/), [Tauqeer Ahmad](https://www.linkedin.com/in/tauqeerahmad5201/), Yogendrasingh Pawar, [Vidushi Gupta](https://www.linkedin.com/in/vidushi-gupta07/), [Jasleen Sondhi](https://www.linkedin.com/in/jasleen-sondhi/)।

|![Sketchnote by @sketchthedocs https://sketchthedocs.dev](../../translated_images/00-Title.8af36cd35da1ac555b678627fbdc6e320c75f0100876ea41d30ea205d3b08d22.pa.png)|
|:---:|
| ਡਾਟਾ ਸਾਇੰਸ ਸ਼ੁਰੂਆਤੀ ਲਈ - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

### 🌐 ਬਹੁ-ਭਾਸ਼ਾ ਸਹਾਇਤਾ

#### GitHub Action ਰਾਹੀਂ ਸਹਾਇਤ (ਆਟੋਮੈਟਿਕ ਅਤੇ ਹਮੇਸ਼ਾ ਅਪ-ਟੂ-ਡੇਟ)

**ਜੇ ਤੁਸੀਂ ਹੋਰ ਭਾਸ਼ਾਵਾਂ ਵਿੱਚ ਅਨੁਵਾਦ ਕਰਵਾਉਣਾ ਚਾਹੁੰਦੇ ਹੋ, ਸਹਾਇਤ ਪ੍ਰਾਪਤ ਭਾਸ਼ਾਵਾਂ ਦੀ ਸੂਚੀ [ਇੱਥੇ](https://github.com/Azure/co-op-translator/blob/main/getting_started/supported-languages.md) ਦਿੱਤੀ ਗਈ ਹੈ।**

#### ਸਾਡੇ ਸਮੁਦਾਇ ਵਿੱਚ ਸ਼ਾਮਲ ਹੋਵੋ 
[![Azure AI Discord](https://dcbadge.limes.pink/api/server/kzRShWzttr)](https://discord.gg/kzRShWzttr)

# ਕੀ ਤੁਸੀਂ ਵਿਦਿਆਰਥੀ ਹੋ?

ਹੇਠਾਂ ਦਿੱਤੇ ਸਰੋਤਾਂ ਨਾਲ ਸ਼ੁਰੂ ਕਰੋ:

- [Student Hub page](https://docs.microsoft.com/en-gb/learn/student-hub?WT.mc_id=academic-77958-bethanycheum) ਇਸ ਪੇਜ 'ਤੇ, ਤੁਹਾਨੂੰ ਸ਼ੁਰੂਆਤੀ ਸਰੋਤ, ਵਿਦਿਆਰਥੀ ਪੈਕ ਅਤੇ ਮੁਫ਼ਤ ਸਰਟੀਫਿਕੇਟ ਵਾਊਚਰ ਪ੍ਰਾਪਤ ਕਰਨ ਦੇ ਤਰੀਕੇ ਮਿਲਣਗੇ। ਇਹ ਇੱਕ ਪੇਜ ਹੈ ਜਿਸਨੂੰ ਤੁਸੀਂ ਬੁੱਕਮਾਰਕ ਕਰਨਾ ਚਾਹੁੰਦੇ ਹੋ ਅਤੇ ਸਮੇਂ-ਸਮੇਂ 'ਤੇ ਚੈੱਕ ਕਰਨਾ ਚਾਹੁੰਦੇ ਹੋ ਕਿਉਂਕਿ ਅਸੀਂ ਘੱਟੋ-ਘੱਟ ਮਹੀਨਾਵਾਰ ਸਮੱਗਰੀ ਬਦਲਦੇ ਹਾਂ।
- [Microsoft Learn Student Ambassadors](https://studentambassadors.microsoft.com?WT.mc_id=academic-77958-bethanycheum) ਵਿਦਿਆਰਥੀ ਅੰਬੈਸਡਰਾਂ ਦੇ ਗਲੋਬਲ ਸਮੁਦਾਇ ਵਿੱਚ ਸ਼ਾਮਲ ਹੋਵੋ, ਇਹ ਮਾਈਕਰੋਸਾਫਟ ਵਿੱਚ ਤੁਹਾਡਾ ਰਸਤਾ ਹੋ ਸਕਦਾ ਹੈ।

# ਸ਼ੁਰੂਆਤ ਕਰਨਾ

> **ਅਧਿਆਪਕਾਂ**: ਅਸੀਂ [ਕੁਝ ਸੁਝਾਅ ਸ਼ਾਮਲ ਕੀਤੇ ਹਨ](for-teachers.md) ਕਿ ਇਸ ਪਾਠਕ੍ਰਮ ਨੂੰ ਕਿਵੇਂ ਵਰਤਣਾ ਹੈ।  ਅਸੀਂ ਤੁਹਾਡਾ ਫੀਡਬੈਕ [ਸਾਡੇ ਚਰਚਾ ਫੋਰਮ](https://github.com/microsoft/Data-Science-For-Beginners/discussions) ਵਿੱਚ ਚਾਹੁੰਦੇ ਹਾਂ!

> **[ਵਿਦਿਆਰਥੀ](https://aka.ms/student-page)**: ਇਸ ਪਾਠਕ੍ਰਮ ਨੂੰ ਆਪਣੇ ਆਪ ਵਰਤਣ ਲਈ, ਪੂਰੇ ਰਿਪੋ ਨੂੰ ਫੋਰਕ ਕਰੋ ਅਤੇ ਆਪਣੇ ਆਪ ਅਭਿਆਸ ਪੂਰੇ ਕਰੋ, ਪਾਠ ਤੋਂ ਪਹਿਲਾਂ ਦੇ ਪ੍ਰਸ਼ਨ ਨਾਲ ਸ਼ੁਰੂ ਕਰਦੇ ਹੋਏ।  ਫਿਰ ਪਾਠ ਪੜ੍ਹੋ ਅਤੇ ਬਾਕੀ ਗਤੀਵਿਧੀਆਂ ਪੂਰੀਆਂ ਕਰੋ। ਪਾਠਾਂ ਨੂੰ ਸਮਝ ਕੇ ਪ੍ਰੋਜੈਕਟ ਬਣਾਉਣ ਦੀ ਕੋਸ਼ਿਸ਼ ਕਰੋ ਨਾ ਕਿ ਹੱਲ ਕੋਡ ਨੂੰ ਕਾਪੀ ਕਰਨ ਦੀ; ਹਾਲਾਂਕਿ, ਉਹ ਕੋਡ /solutions ਫੋਲਡਰ ਵਿੱਚ ਪ੍ਰੋਜੈਕਟ-ਅਧਾਰਤ ਪਾਠਾਂ ਵਿੱਚ ਉਪਲਬਧ ਹੈ। ਇੱਕ ਹੋਰ ਵਿਚਾਰ ਇਹ ਹੋ ਸਕਦਾ ਹੈ ਕਿ ਦੋਸਤਾਂ ਨਾਲ ਇੱਕ ਅਧਿਐਨ ਸਮੂਹ ਬਣਾਓ ਅਤੇ ਸਮੱਗਰੀ ਨੂੰ ਇਕੱਠੇ ਪੜ੍ਹੋ। ਹੋਰ ਅਧਿਐਨ ਲਈ, ਅਸੀਂ [Microsoft Learn](https://docs.microsoft.com/en-us/users/jenlooper-2911/collections/qprpajyoy3x0g7?WT.mc_id=academic-77958-bethanycheum) ਦੀ ਸਿਫਾਰਸ਼ ਕਰਦੇ ਹਾਂ।

## ਟੀਮ ਨਾਲ ਮਿਲੋ

[![Promo video](../../ds-for-beginners.gif)](https://youtu.be/8mzavjQSMM4 "Promo video")

**Gif by** [Mohit Jaisal](https://www.linkedin.com/in/mohitjaisal)

> 🎥 ਉਪਰੋਕਤ ਚਿੱਤਰ 'ਤੇ ਕਲਿਕ ਕਰੋ ਪ੍ਰੋਜੈਕਟ ਅਤੇ ਉਹ ਲੋਕਾਂ ਬਾਰੇ ਵੀਡੀਓ ਦੇਖਣ ਲਈ ਜਿਨ੍ਹਾਂ ਨੇ ਇਸਨੂੰ ਬਣਾਇਆ!

## ਪੈਡਾਗੌਜੀ

ਅਸੀਂ ਇਸ ਪਾਠਕ੍ਰਮ ਨੂੰ ਬਣਾਉਣ ਦੌਰਾਨ ਦੋ ਪੈਡਾਗੌਜੀਕਲ ਸਿਧਾਂਤਾਂ ਨੂੰ ਚੁਣਿਆ ਹੈ: ਇਹ ਯਕੀਨੀ ਬਣਾਉਣਾ ਕਿ ਇਹ ਪ੍ਰੋਜੈਕਟ-ਅਧਾਰਤ ਹੈ ਅਤੇ ਇਹ ਵਾਰੰ-ਵਾਰ ਪ੍ਰਸ਼ਨ ਸ਼ਾਮਲ ਕਰਦਾ ਹੈ। ਇਸ ਸਿਰੀਜ਼ ਦੇ ਅੰਤ ਤੱਕ, ਵਿਦਿਆਰਥੀ ਡਾਟਾ ਸਾਇੰਸ ਦੇ ਮੂਲ ਸਿਧਾਂਤਾਂ ਸਿੱਖ ਚੁੱਕੇ ਹੋਣਗੇ, ਜਿਸ ਵਿੱਚ ਨੈਤਿਕ ਧਾਰਨਾਵਾਂ, ਡਾਟਾ ਤਿਆਰੀ, ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨ ਦੇ ਵੱਖ-ਵੱਖ ਤਰੀਕੇ, ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ, ਡਾਟਾ ਵਿਸ਼ਲੇਸ਼ਣ, ਡਾਟਾ ਸਾਇੰਸ ਦੇ ਅਸਲ-ਜਗਤ ਦੇ ਉਪਯੋਗ ਅਤੇ ਹੋਰ ਬਹੁਤ ਕੁਝ ਸ਼ਾਮਲ ਹਨ।

ਇਸਦੇ ਇਲਾਵਾ, ਕਲਾਸ ਤੋਂ ਪਹਿਲਾਂ ਇੱਕ ਘੱਟ-ਦਬਾਅ ਵਾਲਾ ਪ੍ਰਸ਼ਨ ਵਿਦਿਆਰਥੀ ਨੂੰ ਇੱਕ ਵਿਸ਼ੇ ਨੂੰ ਸਿੱਖਣ ਵੱਲ ਧਿਆਨ ਕੇਂਦ੍ਰਿਤ ਕਰਨ ਲਈ ਸੈਟ ਕਰਦਾ ਹੈ, ਜਦਕਿ ਕਲਾਸ ਤੋਂ ਬਾਅਦ ਦੂਜਾ ਪ੍ਰਸ਼ਨ ਹੋਰ ਰਿਟੇਨਸ਼ਨ ਯਕੀਨੀ ਬਣਾਉਂਦਾ ਹੈ। ਇਹ ਪਾਠਕ੍ਰਮ ਲਚਕੀਲਾ ਅਤੇ ਮਜ਼ੇਦਾਰ ਬਣਾਇਆ ਗਿਆ ਹੈ ਅਤੇ ਇਸਨੂੰ ਪੂਰੇ ਜਾਂ ਅੰਸ਼ਿਕ ਤੌਰ 'ਤੇ ਲਿਆ ਜਾ ਸਕਦਾ ਹੈ। ਪ੍ਰੋਜੈਕਟ ਛੋਟੇ ਸ਼ੁਰੂ ਹੁੰਦੇ ਹਨ ਅਤੇ 10 ਹਫ਼ਤਿਆਂ ਦੇ ਚੱਕਰ ਦੇ ਅੰਤ ਤੱਕ ਵਧਦੇ ਹੀ ਜਟਿਲ ਹੋ ਜਾਂਦੇ ਹਨ।
> ਸਾਡਾ [Code of Conduct](CODE_OF_CONDUCT.md), [Contributing](CONTRIBUTING.md), [Translation](TRANSLATIONS.md) ਦਿਸ਼ਾ-ਨਿਰਦੇਸ਼ ਵੇਖੋ। ਅਸੀਂ ਤੁਹਾਡੀ ਰਚਨਾਤਮਕ ਪ੍ਰਤੀਕ੍ਰਿਆ ਦਾ ਸਵਾਗਤ ਕਰਦੇ ਹਾਂ!
## ਹਰ ਪਾਠ ਵਿੱਚ ਸ਼ਾਮਲ ਹੈ:

- ਵਿਕਲਪਿਕ ਸਕੈਚਨੋਟ
- ਵਿਕਲਪਿਕ ਸਹਾਇਕ ਵੀਡੀਓ
- ਪਾਠ ਤੋਂ ਪਹਿਲਾਂ ਵਾਰਮਅਪ ਕਵਿਜ਼
- ਲਿਖਤ ਪਾਠ
- ਪ੍ਰੋਜੈਕਟ-ਅਧਾਰਿਤ ਪਾਠਾਂ ਲਈ, ਪ੍ਰੋਜੈਕਟ ਬਣਾਉਣ ਲਈ ਕਦਮ-ਦਰ-ਕਦਮ ਗਾਈਡ
- ਗਿਆਨ ਦੀ ਜਾਂਚ
- ਇੱਕ ਚੁਣੌਤੀ
- ਸਹਾਇਕ ਪੜ੍ਹਾਈ
- ਅਸਾਈਨਮੈਂਟ
- [ਪਾਠ ਤੋਂ ਬਾਅਦ ਕਵਿਜ਼](https://ff-quizzes.netlify.app/en/)

> **ਕਵਿਜ਼ਾਂ ਬਾਰੇ ਇੱਕ ਨੋਟ**: ਸਾਰੀਆਂ ਕਵਿਜ਼ਾਂ `Quiz-App` ਫੋਲਡਰ ਵਿੱਚ ਸ਼ਾਮਲ ਹਨ, ਜੋ ਕਿ ਕੁੱਲ 40 ਕਵਿਜ਼ਾਂ ਹਨ, ਹਰ ਇੱਕ ਵਿੱਚ ਤਿੰਨ ਪ੍ਰਸ਼ਨ ਹਨ। ਇਹ ਪਾਠਾਂ ਵਿੱਚੋਂ ਲਿੰਕ ਕੀਤੀਆਂ ਗਈਆਂ ਹਨ, ਪਰ ਕਵਿਜ਼ ਐਪ ਨੂੰ ਸਥਾਨਕ ਤੌਰ 'ਤੇ ਚਲਾਇਆ ਜਾ ਸਕਦਾ ਹੈ ਜਾਂ Azure 'ਤੇ ਡਿਪਲੌਇ ਕੀਤਾ ਜਾ ਸਕਦਾ ਹੈ; `quiz-app` ਫੋਲਡਰ ਵਿੱਚ ਦਿੱਤੇ ਨਿਰਦੇਸ਼ਾਂ ਦੀ ਪਾਲਣਾ ਕਰੋ। ਇਹ ਹੌਲੀ-ਹੌਲੀ ਸਥਾਨਕ ਭਾਸ਼ਾਵਾਂ ਵਿੱਚ ਅਨੁਵਾਦ ਕੀਤੀਆਂ ਜਾ ਰਹੀਆਂ ਹਨ।

## ਪਾਠ

|![ @sketchthedocs ਦੁਆਰਾ ਸਕੈਚਨੋਟ https://sketchthedocs.dev](../../translated_images/00-Roadmap.4905d6567dff47532b9bfb8e0b8980fc6b0b1292eebb24181c1a9753b33bc0f5.pa.png)|
|:---:|
| ਸ਼ੁਰੂਆਤੀ ਡਾਟਾ ਸਾਇੰਸ: ਰੋਡਮੈਪ - _[@nitya](https://twitter.com/nitya) ਦੁਆਰਾ ਸਕੈਚਨੋਟ_ |

| ਪਾਠ ਨੰਬਰ | ਵਿਸ਼ਾ | ਪਾਠ ਸਮੂਹ | ਸਿੱਖਣ ਦੇ ਉਦੇਸ਼ | ਲਿੰਕ ਕੀਤਾ ਪਾਠ | ਲੇਖਕ |
| :-----------: | :----------------------------------------: | :--------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: | :----: |
| 01 | ਡਾਟਾ ਸਾਇੰਸ ਦੀ ਪਰਿਭਾਸ਼ਾ | [ਪ੍ਰਸਤਾਵਨਾ](1-Introduction/README.md) | ਡਾਟਾ ਸਾਇੰਸ ਦੇ ਮੁੱਢਲੇ ਸੰਕਲਪਾਂ ਨੂੰ ਸਿੱਖੋ ਅਤੇ ਇਹ ਕਿਵੇਂ ਕ੍ਰਿਤਮ ਬੁੱਧੀ, ਮਸ਼ੀਨ ਲਰਨਿੰਗ ਅਤੇ ਵੱਡੇ ਡਾਟਾ ਨਾਲ ਸੰਬੰਧਿਤ ਹੈ। | [ਪਾਠ](1-Introduction/01-defining-data-science/README.md) [ਵੀਡੀਓ](https://youtu.be/beZ7Mb_oz9I) | [Dmitry](http://soshnikov.com) |
| 02 | ਡਾਟਾ ਸਾਇੰਸ ਨੈਤਿਕਤਾ | [ਪ੍ਰਸਤਾਵਨਾ](1-Introduction/README.md) | ਡਾਟਾ ਨੈਤਿਕਤਾ ਦੇ ਸੰਕਲਪ, ਚੁਣੌਤੀਆਂ ਅਤੇ ਫਰੇਮਵਰਕ। | [ਪਾਠ](1-Introduction/02-ethics/README.md) | [Nitya](https://twitter.com/nitya) |
| 03 | ਡਾਟਾ ਦੀ ਪਰਿਭਾਸ਼ਾ | [ਪ੍ਰਸਤਾਵਨਾ](1-Introduction/README.md) | ਡਾਟਾ ਕਿਵੇਂ ਵਰਗਬੱਧ ਕੀਤਾ ਜਾਂਦਾ ਹੈ ਅਤੇ ਇਸਦੇ ਆਮ ਸਰੋਤ। | [ਪਾਠ](1-Introduction/03-defining-data/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 04 | ਅੰਕੜੇ ਅਤੇ ਸੰਭਾਵਨਾ ਦਾ ਪਰਿਚਯ | [ਪ੍ਰਸਤਾਵਨਾ](1-Introduction/README.md) | ਡਾਟਾ ਨੂੰ ਸਮਝਣ ਲਈ ਸੰਭਾਵਨਾ ਅਤੇ ਅੰਕੜੇ ਦੇ ਗਣਿਤਕ ਤਕਨੀਕਾਂ। | [ਪਾਠ](1-Introduction/04-stats-and-probability/README.md) [ਵੀਡੀਓ](https://youtu.be/Z5Zy85g4Yjw) | [Dmitry](http://soshnikov.com) |
| 05 | ਰਿਲੇਸ਼ਨਲ ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ | [ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ](2-Working-With-Data/README.md) | ਰਿਲੇਸ਼ਨਲ ਡਾਟਾ ਦਾ ਪਰਿਚਯ ਅਤੇ ਸਟ੍ਰਕਚਰਡ ਕਵੈਰੀ ਲੈਂਗਵੇਜ (SQL) ਨਾਲ ਰਿਲੇਸ਼ਨਲ ਡਾਟਾ ਦੀ ਜਾਂਚ ਅਤੇ ਵਿਸ਼ਲੇਸ਼ਣ ਦੇ ਮੁੱਢਲੇ ਸਿਧਾਂਤ। | [ਪਾਠ](2-Working-With-Data/05-relational-databases/README.md) | [Christopher](https://www.twitter.com/geektrainer) | | |
| 06 | NoSQL ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ | [ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ](2-Working-With-Data/README.md) | ਗੈਰ-ਰਿਲੇਸ਼ਨਲ ਡਾਟਾ ਦਾ ਪਰਿਚਯ, ਇਸਦੇ ਵੱਖ-ਵੱਖ ਪ੍ਰਕਾਰ ਅਤੇ ਦਸਤਾਵੇਜ਼ ਡਾਟਾਬੇਸ ਦੀ ਜਾਂਚ ਅਤੇ ਵਿਸ਼ਲੇਸ਼ਣ ਦੇ ਮੁੱਢਲੇ ਸਿਧਾਂਤ। | [ਪਾਠ](2-Working-With-Data/06-non-relational/README.md) | [Jasmine](https://twitter.com/paladique)|
| 07 | Python ਨਾਲ ਕੰਮ ਕਰਨਾ | [ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ](2-Working-With-Data/README.md) | Pandas ਵਰਗੀਆਂ ਲਾਇਬ੍ਰੇਰੀਆਂ ਨਾਲ ਡਾਟਾ ਦੀ ਜਾਂਚ ਲਈ Python ਦੀ ਵਰਤੋਂ ਦੇ ਮੁੱਢਲੇ ਸਿਧਾਂਤ। Python ਪ੍ਰੋਗਰਾਮਿੰਗ ਦੀ ਬੁਨਿਆਦੀ ਸਮਝ ਸਿਫਾਰਸ਼ੀ ਹੈ। | [ਪਾਠ](2-Working-With-Data/07-python/README.md) [ਵੀਡੀਓ](https://youtu.be/dZjWOGbsN4Y) | [Dmitry](http://soshnikov.com) |
| 08 | ਡਾਟਾ ਤਿਆਰੀ | [ਡਾਟਾ ਨਾਲ ਕੰਮ ਕਰਨਾ](2-Working-With-Data/README.md) | ਗੁੰਝਲਦਾਰ, ਗਲਤ ਜਾਂ ਅਧੂਰੇ ਡਾਟਾ ਨੂੰ ਹੱਲ ਕਰਨ ਲਈ ਡਾਟਾ ਨੂੰ ਸਾਫ ਕਰਨ ਅਤੇ ਰੂਪਾਂਤਰਿਤ ਕਰਨ ਦੀਆਂ ਤਕਨੀਕਾਂ। | [ਪਾਠ](2-Working-With-Data/08-data-preparation/README.md) | [Jasmine](https://www.twitter.com/paladique) |
| 09 | ਮਾਤਰਾ ਦੀ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ | [ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ](3-Data-Visualization/README.md) | Matplotlib ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਪੰਛੀਆਂ ਦੇ ਡਾਟਾ ਨੂੰ ਵਿਜ਼ੁਅਲਾਈਜ਼ ਕਰਨਾ ਸਿੱਖੋ 🦆 | [ਪਾਠ](3-Data-Visualization/09-visualization-quantities/README.md) | [Jen](https://twitter.com/jenlooper) |
| 10 | ਡਾਟਾ ਦੇ ਵੰਡ ਦੀ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ | [ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ](3-Data-Visualization/README.md) | ਇੱਕ ਅੰਤਰਾਲ ਵਿੱਚ ਅਵਲੋਕਨ ਅਤੇ ਰੁਝਾਨਾਂ ਨੂੰ ਵਿਜ਼ੁਅਲਾਈਜ਼ ਕਰਨਾ। | [ਪਾਠ](3-Data-Visualization/10-visualization-distributions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 11 | ਅਨੁਪਾਤਾਂ ਦੀ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ | [ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ](3-Data-Visualization/README.md) | ਵਿਸ਼ੇਸ਼ ਅਤੇ ਸਮੂਹਬੱਧ ਪ੍ਰਤੀਸ਼ਤਾਂ ਨੂੰ ਵਿਜ਼ੁਅਲਾਈਜ਼ ਕਰਨਾ। | [ਪਾਠ](3-Data-Visualization/11-visualization-proportions/README.md) | [Jen](https://twitter.com/jenlooper) |
| 12 | ਸੰਬੰਧਾਂ ਦੀ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ | [ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ](3-Data-Visualization/README.md) | ਡਾਟਾ ਦੇ ਸੈੱਟਾਂ ਅਤੇ ਉਨ੍ਹਾਂ ਦੇ ਵੈਰੀਏਬਲਾਂ ਦੇ ਵਿਚਕਾਰ ਸੰਬੰਧਾਂ ਅਤੇ ਸਹਸੰਬੰਧਾਂ ਨੂੰ ਵਿਜ਼ੁਅਲਾਈਜ਼ ਕਰਨਾ। | [ਪਾਠ](3-Data-Visualization/12-visualization-relationships/README.md) | [Jen](https://twitter.com/jenlooper) |
| 13 | ਅਰਥਪੂਰਨ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ | [ਡਾਟਾ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ](3-Data-Visualization/README.md) | ਸਮੱਸਿਆ ਹੱਲ ਕਰਨ ਅਤੇ ਅੰਤਰਦ੍ਰਿਸ਼ਟੀ ਲਈ ਤੁਹਾਡੇ ਵਿਜ਼ੁਅਲਾਈਜ਼ੇਸ਼ਨ ਨੂੰ ਮੁੱਲਵਾਨ ਬਣਾਉਣ ਲਈ ਤਕਨੀਕਾਂ ਅਤੇ ਮਾਰਗਦਰਸ਼ਨ। | [ਪਾਠ](3-Data-Visualization/13-meaningful-visualizations/README.md) | [Jen](https://twitter.com/jenlooper) |
| 14 | ਡਾਟਾ ਸਾਇੰਸ ਲਾਈਫਸਾਈਕਲ ਦਾ ਪਰਿਚਯ | [ਲਾਈਫਸਾਈਕਲ](4-Data-Science-Lifecycle/README.md) | ਡਾਟਾ ਸਾਇੰਸ ਲਾਈਫਸਾਈਕਲ ਦਾ ਪਰਿਚਯ ਅਤੇ ਡਾਟਾ ਪ੍ਰਾਪਤ ਕਰਨ ਅਤੇ ਕੱਢਣ ਦਾ ਪਹਿਲਾ ਕਦਮ। | [ਪਾਠ](4-Data-Science-Lifecycle/14-Introduction/README.md) | [Jasmine](https://twitter.com/paladique) |
| 15 | ਵਿਸ਼ਲੇਸ਼ਣ | [ਲਾਈਫਸਾਈਕਲ](4-Data-Science-Lifecycle/README.md) | ਡਾਟਾ ਸਾਇੰਸ ਲਾਈਫਸਾਈਕਲ ਦਾ ਇਹ ਚਰਨ ਡਾਟਾ ਨੂੰ ਵਿਸ਼ਲੇਸ਼ਣ ਕਰਨ ਦੀਆਂ ਤਕਨੀਕਾਂ 'ਤੇ ਧਿਆਨ ਕੇਂਦ੍ਰਿਤ ਕਰਦਾ ਹੈ। | [ਪਾਠ](4-Data-Science-Lifecycle/15-analyzing/README.md) | [Jasmine](https://twitter.com/paladique) | | |
| 16 | ਸੰਚਾਰ | [ਲਾਈਫਸਾਈਕਲ](4-Data-Science-Lifecycle/README.md) | ਡਾਟਾ ਤੋਂ ਪ੍ਰਾਪਤ ਅੰਤਰਦ੍ਰਿਸ਼ਟੀ ਨੂੰ ਇਸ ਤਰੀਕੇ ਨਾਲ ਪੇਸ਼ ਕਰਨ 'ਤੇ ਧਿਆਨ ਕੇਂਦ੍ਰਿਤ ਕਰਦਾ ਹੈ ਜੋ ਫੈਸਲੇ ਕਰਨ ਵਾਲਿਆਂ ਲਈ ਸਮਝਣਾ ਆਸਾਨ ਬਣਾਉਂਦਾ ਹੈ। | [ਪਾਠ](4-Data-Science-Lifecycle/16-communication/README.md) | [Jalen](https://twitter.com/JalenMcG) | | |
| 17 | ਕਲਾਉਡ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ | [ਕਲਾਉਡ ਡਾਟਾ](5-Data-Science-In-Cloud/README.md) | ਕਲਾਉਡ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ ਅਤੇ ਇਸਦੇ ਫਾਇਦਿਆਂ ਦਾ ਪਰਿਚਯ। | [ਪਾਠ](5-Data-Science-In-Cloud/17-Introduction/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) ਅਤੇ [Maud](https://twitter.com/maudstweets) |
| 18 | ਕਲਾਉਡ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ | [ਕਲਾਉਡ ਡਾਟਾ](5-Data-Science-In-Cloud/README.md) | ਲੋ ਕੋਡ ਟੂਲਜ਼ ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਮਾਡਲਾਂ ਨੂੰ ਟ੍ਰੇਨ ਕਰਨਾ। |[ਪਾਠ](5-Data-Science-In-Cloud/18-Low-Code/README.md) | [Tiffany](https://twitter.com/TiffanySouterre) ਅਤੇ [Maud](https://twitter.com/maudstweets) |
| 19 | ਕਲਾਉਡ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ | [ਕਲਾਉਡ ਡਾਟਾ](5-Data-Science-In-Cloud/README.md) | Azure Machine Learning Studio ਨਾਲ ਮਾਡਲਾਂ ਨੂੰ ਡਿਪਲੌਇ ਕਰਨਾ। | [ਪਾਠ](5-Data-Science-In-Cloud/19-Azure/README.md)| [Tiffany](https://twitter.com/TiffanySouterre) ਅਤੇ [Maud](https://twitter.com/maudstweets) |
| 20 | ਜੰਗਲੀ ਹਾਲਾਤਾਂ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ | [ਜੰਗਲੀ ਹਾਲਾਤ](6-Data-Science-In-Wild/README.md) | ਅਸਲ ਦੁਨੀਆ ਵਿੱਚ ਡਾਟਾ ਸਾਇੰਸ ਚਲਿਤ ਪ੍ਰੋਜੈਕਟ। | [ਪਾਠ](6-Data-Science-In-Wild/20-Real-World-Examples/README.md) | [Nitya](https://twitter.com/nitya) |

## GitHub Codespaces

ਇਸ ਸੈਂਪਲ ਨੂੰ Codespace ਵਿੱਚ ਖੋਲ੍ਹਣ ਲਈ ਇਹ ਕਦਮ ਅਨੁਸਰਣ ਕਰੋ:
1. Code ਡ੍ਰੌਪ-ਡਾਊਨ ਮੀਨੂ 'ਤੇ ਕਲਿੱਕ ਕਰੋ ਅਤੇ Open with Codespaces ਵਿਕਲਪ ਚੁਣੋ।
2. ਪੈਨ ਦੇ ਹੇਠਾਂ + New codespace ਚੁਣੋ।
ਹੋਰ ਜਾਣਕਾਰੀ ਲਈ, [GitHub ਦਸਤਾਵੇਜ਼](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace) ਦੀ ਜਾਂਚ ਕਰੋ।

## VSCode ਰਿਮੋਟ - ਕੰਟੇਨਰ
ਇਹ ਕਦਮ ਅਨੁਸਰਣ ਕਰੋ ਤਾਂ ਜੋ ਤੁਸੀਂ ਆਪਣੇ ਸਥਾਨਕ ਮਸ਼ੀਨ ਅਤੇ VSCode ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਇਸ ਰਿਪੋ ਨੂੰ ਇੱਕ ਕੰਟੇਨਰ ਵਿੱਚ ਖੋਲ੍ਹ ਸਕੋ, VS Code Remote - Containers ਐਕਸਟੈਂਸ਼ਨ ਦੀ ਵਰਤੋਂ ਕਰਦੇ ਹੋਏ:

1. ਜੇ ਇਹ ਪਹਿਲੀ ਵਾਰ ਹੈ ਕਿ ਤੁਸੀਂ ਵਿਕਾਸ ਕੰਟੇਨਰ ਦੀ ਵਰਤੋਂ ਕਰ ਰਹੇ ਹੋ, ਤਾਂ ਕਿਰਪਾ ਕਰਕੇ ਯਕੀਨੀ ਬਣਾਓ ਕਿ ਤੁਹਾਡੀ ਸਿਸਟਮ [ਸ਼ੁਰੂਆਤੀ ਦਸਤਾਵੇਜ਼](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started) ਵਿੱਚ ਦਿੱਤੇ ਪ੍ਰੀ-ਰਿਕਵਾਇਰਮੈਂਟਾਂ ਨੂੰ ਪੂਰਾ ਕਰਦੀ ਹੈ (ਜਿਵੇਂ ਕਿ Docker ਇੰਸਟਾਲ ਕੀਤਾ ਹੋਵੇ)।

ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਦੀ ਵਰਤੋਂ ਕਰਨ ਲਈ, ਤੁਸੀਂ ਇਸਨੂੰ ਇੱਕ ਅਲੱਗ Docker ਵਾਲਿਊਮ ਵਿੱਚ ਖੋਲ੍ਹ ਸਕਦੇ ਹੋ:

**ਨੋਟ**: ਇਸਦੇ ਪਿੱਛੇ, ਇਹ Remote-Containers: **Clone Repository in Container Volume...** ਕਮਾਂਡ ਦੀ ਵਰਤੋਂ ਕਰੇਗਾ ਤਾਂ ਜੋ ਸਥਾਨਕ ਫਾਈਲ ਸਿਸਟਮ ਦੀ ਬਜਾਏ Docker ਵਾਲਿਊਮ ਵਿੱਚ ਸੋਰ ਕੋਡ ਨੂੰ ਕਲੋਨ ਕੀਤਾ ਜਾ ਸਕੇ। [ਵਾਲਿਊਮ](https://docs.docker.com/storage/volumes/) ਡਾਟਾ ਨੂੰ ਸਥਿਰ ਕਰਨ ਲਈ ਪਸੰਦੀਦਾ ਮਕੈਨਿਜ਼ਮ ਹਨ।

ਜਾਂ ਸਥਾਨਕ ਤੌਰ 'ਤੇ ਕਲੋਨ ਕੀਤੇ ਜਾਂ ਡਾਊਨਲੋਡ ਕੀਤੇ ਰਿਪੋਜ਼ਟਰੀ ਦੇ ਵਰਜਨ ਨੂੰ ਖੋਲ੍ਹੋ:

- ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਨੂੰ ਆਪਣੇ ਸਥਾਨਕ ਫਾਈਲ ਸਿਸਟਮ 'ਤੇ ਕਲੋਨ ਕਰੋ।
- F1 ਦਬਾਓ ਅਤੇ **Remote-Containers: Open Folder in Container...** ਕਮਾਂਡ ਚੁਣੋ।
- ਇਸ ਫੋਲਡਰ ਦੀ ਕਲੋਨ ਕੀਤੀ ਕਾਪੀ ਚੁਣੋ, ਕੰਟੇਨਰ ਨੂੰ ਸ਼ੁਰੂ ਕਰਨ ਦੀ ਉਡੀਕ ਕਰੋ, ਅਤੇ ਚੀਜ਼ਾਂ ਨੂੰ ਅਜ਼ਮਾਓ।

## ਆਫਲਾਈਨ ਪਹੁੰਚ

ਤੁਸੀਂ [Docsify](https://docsify.js.org/#/) ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਇਸ ਦਸਤਾਵੇਜ਼ ਨੂੰ ਆਫਲਾਈਨ ਚਲਾ ਸਕਦੇ ਹੋ। ਇਸ ਰਿਪੋ ਨੂੰ ਫੋਰਕ ਕਰੋ, [Docsify ਇੰਸਟਾਲ ਕਰੋ](https://docsify.js.org/#/quickstart) ਆਪਣੇ ਸਥਾਨਕ ਮਸ਼ੀਨ 'ਤੇ, ਫਿਰ ਇਸ ਰਿਪੋ ਦੇ ਰੂਟ ਫੋਲਡਰ ਵਿੱਚ `docsify serve` ਟਾਈਪ ਕਰੋ। ਵੈਬਸਾਈਟ ਤੁਹਾਡੇ localhost `localhost:3000` 'ਤੇ ਪੋਰਟ 3000 'ਤੇ ਸਰਵ ਕੀਤੀ ਜਾਵੇਗੀ।

> ਨੋਟ, ਨੋਟਬੁੱਕ Docsify ਦੁਆਰਾ ਰੈਂਡਰ ਨਹੀਂ ਕੀਤੀਆਂ ਜਾਣਗੀਆਂ, ਇਸ ਲਈ ਜਦੋਂ ਤੁਹਾਨੂੰ ਨੋਟਬੁੱਕ ਚਲਾਉਣ ਦੀ ਲੋੜ ਹੋਵੇ, ਤਾਂ ਇਸਨੂੰ Python kernel ਚਲਾਉਣ ਵਾਲੇ VS Code ਵਿੱਚ ਅਲੱਗ ਕਰਕੇ ਚਲਾਓ।

## ਹੋਰ ਪਾਠਕ੍ਰਮ

ਸਾਡੀ ਟੀਮ ਹੋਰ ਪਾਠਕ੍ਰਮ ਤਿਆਰ ਕਰਦੀ ਹੈ! ਚੈੱਕ ਕਰੋ:

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
- [XR Development for Beginners](

---

**ਅਸਵੀਕਾਰਨਾ**:  
ਇਹ ਦਸਤਾਵੇਜ਼ AI ਅਨੁਵਾਦ ਸੇਵਾ [Co-op Translator](https://github.com/Azure/co-op-translator) ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਅਨੁਵਾਦ ਕੀਤਾ ਗਿਆ ਹੈ। ਜਦੋਂ ਕਿ ਅਸੀਂ ਸਹੀਤਾ ਲਈ ਯਤਨਸ਼ੀਲ ਹਾਂ, ਕਿਰਪਾ ਕਰਕੇ ਧਿਆਨ ਦਿਓ ਕਿ ਸਵੈਚਾਲਿਤ ਅਨੁਵਾਦਾਂ ਵਿੱਚ ਗਲਤੀਆਂ ਜਾਂ ਅਸੁਚਨਾਵਾਂ ਹੋ ਸਕਦੀਆਂ ਹਨ। ਮੂਲ ਦਸਤਾਵੇਜ਼, ਜੋ ਇਸਦੀ ਮੂਲ ਭਾਸ਼ਾ ਵਿੱਚ ਹੈ, ਨੂੰ ਅਧਿਕਾਰਤ ਸਰੋਤ ਮੰਨਿਆ ਜਾਣਾ ਚਾਹੀਦਾ ਹੈ। ਮਹੱਤਵਪੂਰਨ ਜਾਣਕਾਰੀ ਲਈ, ਪੇਸ਼ੇਵਰ ਮਨੁੱਖੀ ਅਨੁਵਾਦ ਦੀ ਸਿਫਾਰਸ਼ ਕੀਤੀ ਜਾਂਦੀ ਹੈ। ਇਸ ਅਨੁਵਾਦ ਦੀ ਵਰਤੋਂ ਤੋਂ ਪੈਦਾ ਹੋਣ ਵਾਲੇ ਕਿਸੇ ਵੀ ਗਲਤਫਹਿਮੀ ਜਾਂ ਗਲਤ ਵਿਆਖਿਆ ਲਈ ਅਸੀਂ ਜ਼ਿੰਮੇਵਾਰ ਨਹੀਂ ਹਾਂ।