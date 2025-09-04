<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "90a815d332aea41a222f4c6372e7186e",
  "translation_date": "2025-09-04T16:59:40+00:00",
  "source_file": "2-Working-With-Data/08-data-preparation/README.md",
  "language_code": "ne"
}
-->
# डेटा संग काम गर्ने: डेटा तयारी

|![ [(@sketchthedocs)](https://sketchthedocs.dev) द्वारा स्केच नोट ](../../sketchnotes/08-DataPreparation.png)|
|:---:|
|डेटा तयारी - _[@nitya](https://twitter.com/nitya) द्वारा स्केच नोट_ |

## [पूर्व-व्याख्यान क्विज](https://purple-hill-04aebfb03.1.azurestaticapps.net/quiz/14)

डेटाको स्रोत अनुसार, कच्चा डेटा केही असंगतिहरू समावेश गर्न सक्छ जसले विश्लेषण र मोडलिङमा चुनौतीहरू सिर्जना गर्दछ। अर्को शब्दमा, यस्तो डेटा "फोहोर" मान्न सकिन्छ र यसलाई सफा गर्न आवश्यक हुन्छ। यो पाठले हराएको, गलत, वा अपूर्ण डेटा सम्बोधन गर्न डेटा सफा गर्ने र परिवर्तन गर्ने प्रविधिहरूमा केन्द्रित छ। यस पाठमा समेटिएका विषयहरू Python र Pandas लाइब्रेरी प्रयोग गरेर [यस निर्देशिकाको नोटबुकमा](notebook.ipynb) प्रदर्शन गरिनेछ।

## डेटा सफा गर्ने महत्त्व

- **प्रयोग र पुनःप्रयोगको सजिलो**: जब डेटा राम्रोसँग व्यवस्थित र सामान्यीकृत हुन्छ, यसलाई खोज्न, प्रयोग गर्न, र अरूसँग साझा गर्न सजिलो हुन्छ।

- **संगतता**: डेटा विज्ञानले प्रायः एकभन्दा बढी डेटासेटसँग काम गर्न आवश्यक पर्दछ, जहाँ विभिन्न स्रोतहरूबाट आएका डेटासेटहरूलाई एकसाथ जोड्नुपर्छ। प्रत्येक व्यक्तिगत डेटासेटमा समान मानकीकरण सुनिश्चित गर्दा, सबै डेटासेटहरू एकसाथ मिल्दा पनि डेटा उपयोगी रहन्छ।

- **मोडलको शुद्धता**: सफा गरिएको डेटा मोडलहरूको शुद्धता सुधार गर्दछ, जुन यसमा निर्भर गर्दछ।

## सामान्य सफा गर्ने लक्ष्यहरू र रणनीतिहरू

- **डेटासेट अन्वेषण**: [पछिल्लो पाठ](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/4-Data-Science-Lifecycle/15-analyzing) मा समेटिएको डेटा अन्वेषणले सफा गर्न आवश्यक डेटा पत्ता लगाउन मद्दत गर्दछ। डेटासेटभित्रका मानहरूलाई दृश्यात्मक रूपमा अवलोकन गर्दा बाँकी भाग कस्तो देखिन्छ भन्ने अपेक्षा सेट गर्न सकिन्छ, वा समाधान गर्न सकिने समस्याहरूको विचार प्रदान गर्न सकिन्छ। अन्वेषणमा आधारभूत क्वेरी, दृश्यात्मकता, र नमूना समावेश हुन सक्छ।

- **फर्म्याटिङ**: स्रोत अनुसार, डेटा प्रस्तुत गर्ने तरिकामा असंगतता हुन सक्छ। यसले डेटासेटभित्र मान देखिए पनि दृश्यात्मकता वा क्वेरी परिणामहरूमा सही रूपमा प्रतिनिधित्व नगरिएको अवस्थामा खोज्न र मान प्रस्तुत गर्न समस्या उत्पन्न गर्न सक्छ। सामान्य फर्म्याटिङ समस्याहरूमा ह्वाइटस्पेस, मिति, र डेटा प्रकार समाधान गर्न समावेश हुन्छ। फर्म्याटिङ समस्याहरू समाधान गर्ने जिम्मेवारी प्रायः डेटा प्रयोग गर्ने व्यक्तिहरूको हुन्छ। उदाहरणका लागि, मिति र संख्याहरू प्रस्तुत गर्ने मानक देश अनुसार फरक हुन सक्छ।

- **डुप्लिकेसन**: डेटा जसको एकभन्दा बढी घटना छ, गलत परिणाम उत्पादन गर्न सक्छ र सामान्यतया हटाउनुपर्छ। यो दुई वा बढी डेटासेटहरू जोड्दा सामान्य घटना हुन सक्छ। तर, केही अवस्थामा, जोडिएका डेटासेटहरूमा डुप्लिकेसनले थप जानकारी प्रदान गर्न सक्छ र यसलाई सुरक्षित राख्न आवश्यक हुन सक्छ।

- **हराएको डेटा**: हराएको डेटा गलत परिणामहरू साथै कमजोर वा पक्षपाती परिणामहरू निम्त्याउन सक्छ। कहिलेकाहीँ यसलाई डेटा पुनःलोड गरेर, Python जस्ता कोड र गणनाको प्रयोग गरेर हराएको मानहरू भर्न, वा केवल मान र सम्बन्धित डेटा हटाएर समाधान गर्न सकिन्छ। डेटा किन र कसरी हरायो भन्ने कारणहरूमा निर्भर गर्दै, हराएको मानहरू समाधान गर्न लिइने कार्यहरू फरक हुन सक्छ।

## DataFrame जानकारी अन्वेषण गर्दै
> **सिक्ने लक्ष्य:** यो उपविभागको अन्त्यसम्ममा, तपाईं pandas DataFrames मा संग्रहित डेटा बारे सामान्य जानकारी पत्ता लगाउन सहज हुनुहुनेछ।

एकपटक तपाईंले pandas मा आफ्नो डेटा लोड गरेपछि, यो सम्भवतः DataFrame मा हुनेछ (पछिल्लो [पाठ](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/2-Working-With-Data/07-python#dataframe) मा विस्तृत अवलोकन हेर्नुहोस्)। तर, यदि तपाईंको DataFrame मा 60,000 पङ्क्तिहरू र 400 स्तम्भहरू छन् भने, तपाईंले काम गरिरहेको डेटा कस्तो छ भनेर कसरी थाहा पाउनुहुन्छ? सौभाग्यवश, [pandas](https://pandas.pydata.org/) ले DataFrame को समग्र जानकारी छिटो हेर्नका लागि केही सुविधाजनक उपकरणहरू प्रदान गर्दछ, साथै पहिलो र अन्तिम केही पङ्क्तिहरू हेर्नका लागि।

यस कार्यक्षमता अन्वेषण गर्न, हामी Python scikit-learn लाइब्रेरी आयात गर्नेछौं र एक प्रसिद्ध डेटासेट प्रयोग गर्नेछौं: **Iris डेटा सेट**।

```python
import pandas as pd
from sklearn.datasets import load_iris

iris = load_iris()
iris_df = pd.DataFrame(data=iris['data'], columns=iris['feature_names'])
```
|                                        |sepal length (cm)|sepal width (cm)|petal length (cm)|petal width (cm)|
|----------------------------------------|-----------------|----------------|-----------------|----------------|
|0                                       |5.1              |3.5             |1.4              |0.2             |
|1                                       |4.9              |3.0             |1.4              |0.2             |
|2                                       |4.7              |3.2             |1.3              |0.2             |
|3                                       |4.6              |3.1             |1.5              |0.2             |
|4                                       |5.0              |3.6             |1.4              |0.2             |

- **DataFrame.info**: सुरु गर्न, `info()` विधि प्रयोग गरेर `DataFrame` मा रहेको सामग्रीको सारांश प्रिन्ट गर्न सकिन्छ। यो डेटासेटमा के छ हेर्नुहोस्:
```python
iris_df.info()
```
```
RangeIndex: 150 entries, 0 to 149
Data columns (total 4 columns):
 #   Column             Non-Null Count  Dtype  
---  ------             --------------  -----  
 0   sepal length (cm)  150 non-null    float64
 1   sepal width (cm)   150 non-null    float64
 2   petal length (cm)  150 non-null    float64
 3   petal width (cm)   150 non-null    float64
dtypes: float64(4)
memory usage: 4.8 KB
```
यसबाट, हामीलाई थाहा हुन्छ कि *Iris* डेटासेटमा चार स्तम्भहरूमा 150 प्रविष्टिहरू छन् र कुनै पनि null प्रविष्टिहरू छैनन्। सबै डेटा 64-बिट फ्लोटिङ-पोइन्ट संख्याहरूको रूपमा संग्रहित छ।

- **DataFrame.head()**: त्यसपछि, `DataFrame` को वास्तविक सामग्री जाँच गर्न, हामी `head()` विधि प्रयोग गर्छौं। हाम्रो `iris_df` को पहिलो केही पङ्क्तिहरू कस्तो देखिन्छ हेर्नुहोस्:
```python
iris_df.head()
```
```
   sepal length (cm)  sepal width (cm)  petal length (cm)  petal width (cm)
0                5.1               3.5                1.4               0.2
1                4.9               3.0                1.4               0.2
2                4.7               3.2                1.3               0.2
3                4.6               3.1                1.5               0.2
4                5.0               3.6                1.4               0.2
```
- **DataFrame.tail()**: उल्टो, `DataFrame` को अन्तिम केही पङ्क्तिहरू जाँच गर्न, हामी `tail()` विधि प्रयोग गर्छौं:
```python
iris_df.tail()
```
```
     sepal length (cm)  sepal width (cm)  petal length (cm)  petal width (cm)
145                6.7               3.0                5.2               2.3
146                6.3               2.5                5.0               1.9
147                6.5               3.0                5.2               2.0
148                6.2               3.4                5.4               2.3
149                5.9               3.0                5.1               1.8
```
> **टेकअवे:** DataFrame मा जानकारीको मेटाडेटा हेर्दा वा पहिलो र अन्तिम केही मानहरू हेर्दा मात्र, तपाईंले काम गरिरहेको डेटा आकार, प्रकार, र सामग्रीको तत्काल विचार प्राप्त गर्न सक्नुहुन्छ।

## हराएको डेटा सम्बोधन गर्दै
> **सिक्ने लक्ष्य:** यो उपविभागको अन्त्यसम्ममा, तपाईं DataFrames बाट null मानहरू प्रतिस्थापन गर्न वा हटाउन जान्नुहुनेछ।

प्रायः तपाईंले प्रयोग गर्न चाहेको (वा प्रयोग गर्नुपर्ने) डेटासेटहरूमा हराएको मानहरू हुन्छन्। हराएको डेटा कसरी सम्बोधन गरिन्छ भन्नेमा सूक्ष्म व्यापार-अफहरू हुन्छन् जसले अन्तिम विश्लेषण र वास्तविक संसारको परिणामहरूमा प्रभाव पार्न सक्छ।

Pandas ले हराएको मानहरू दुई तरिकामा सम्बोधन गर्छ। पहिलो, तपाईंले पहिलेका खण्डहरूमा देख्नुभएको छ: `NaN`, वा Not a Number। यो वास्तवमा IEEE फ्लोटिङ-पोइन्ट विशिष्टताको एक विशेष मान हो र यो केवल हराएको फ्लोटिङ-पोइन्ट मानहरू संकेत गर्न प्रयोग गरिन्छ।

फ्लोटहरू बाहेकका हराएको मानहरूको लागि, pandas ले Python `None` वस्तु प्रयोग गर्छ। जबकि `None` र `NaN` ले मूलतः एउटै कुरा संकेत गर्छन्, यी दुई फरक प्रकारका मानहरू प्रयोग गर्नुको प्रोग्रामिङ कारणहरू छन्। 

`NaN` र `None` को बारेमा थप जानकारी [नोटबुक](https://github.com/microsoft/Data-Science-For-Beginners/blob/main/4-Data-Science-Lifecycle/15-analyzing/notebook.ipynb) बाट हेर्नुहोस्!

- **Null मानहरू पत्ता लगाउँदै**: `pandas` मा, `isnull()` र `notnull()` विधिहरू null डेटा पत्ता लगाउनका लागि मुख्य विधिहरू हुन्। दुवैले Boolean मास्कहरू फिर्ता गर्छन्। हामी `numpy` प्रयोग गरेर `NaN` मानहरू जाँच गर्नेछौं:
```python
import numpy as np

example1 = pd.Series([0, np.nan, '', None])
example1.isnull()
```
```
0    False
1     True
2    False
3     True
dtype: bool
```
आउटपुटलाई ध्यानपूर्वक हेर्नुहोस्। के यसले तपाईंलाई अचम्मित बनायो? `0` एक अंकगणितीय null हो, तर यो पूर्ण रूपमा राम्रो पूर्णांक हो र pandas यसलाई त्यस्तै मान्छ। `''` अलि सूक्ष्म छ। जबकि हामीले यसलाई खण्ड 1 मा खाली स्ट्रिङ मानको रूपमा प्रयोग गर्यौं, यो स्ट्रिङ वस्तु हो र pandas को दृष्टिकोणमा null को प्रतिनिधित्व होइन।

अब, यी विधिहरूलाई व्यावहारिक रूपमा प्रयोग गर्ने तरिकामा प्रयोग गरौं। Boolean मास्कहरूलाई `Series` वा `DataFrame` सूचकांकको रूपमा प्रयोग गर्न सकिन्छ, जुन हराएको (वा उपस्थित) मानहरूसँग काम गर्दा उपयोगी हुन्छ।

> **टेकअवे:** `isnull()` र `notnull()` विधिहरूले `DataFrame` मा समान परिणामहरू उत्पादन गर्छन्: तिनीहरूले परिणामहरू र ती परिणामहरूको सूचकांक देखाउँछन्, जसले तपाईंलाई डेटा व्यवस्थापन गर्दा धेरै मद्दत गर्नेछ।

- **Null मानहरू हटाउँदै**: हराएको मानहरू पहिचान गर्न बाहेक, pandas ले `Series` र `DataFrame` बाट null मानहरू हटाउन सुविधाजनक माध्यम प्रदान गर्दछ। (विशेष गरी ठूला डेटासेटहरूमा, हराएको [NA] मानहरूलाई अन्य तरिकामा सम्बोधन गर्नुभन्दा विश्लेषणबाट हटाउनु अधिक सल्लाहयोग्य हुन्छ।) यो कार्यमा फर्कौं:
```python
example1 = example1.dropna()
example1
```
```
0    0
2     
dtype: object
```
ध्यान दिनुहोस् कि यो तपाईंको `example3[example3.notnull()]` को आउटपुट जस्तै देखिनुपर्छ। यहाँ फरक के छ भने, `dropna` ले हराएको मानहरू `Series` `example1` बाट हटाएको छ।

`DataFrame` दुई आयामहरू भएकोले, यसले डेटा हटाउनका लागि थप विकल्पहरू प्रदान गर्दछ।

```python
example2 = pd.DataFrame([[1,      np.nan, 7], 
                         [2,      5,      8], 
                         [np.nan, 6,      9]])
example2
```
|      | 0 | 1 | 2 |
|------|---|---|---|
|0     |1.0|NaN|7  |
|1     |2.0|5.0|8  |
|2     |NaN|6.0|9  |

(Did you notice that pandas upcast two of the columns to floats to accommodate the `NaN`s?)

You cannot drop a single value from a `DataFrame`, so you have to drop full rows or columns. Depending on what you are doing, you might want to do one or the other, and so pandas gives you options for both. Because in data science, columns generally represent variables and rows represent observations, you are more likely to drop rows of data; the default setting for `dropna()` is to drop all rows that contain any null values:

```python
example2.dropna()
```
```
	0	1	2
1	2.0	5.0	8
```
If necessary, you can drop NA values from columns. Use `axis=1` to do so:
```python
example2.dropna(axis='columns')
```
```
	2
0	7
1	8
2	9
```
Notice that this can drop a lot of data that you might want to keep, particularly in smaller datasets. What if you just want to drop rows or columns that contain several or even just all null values? You specify those setting in `dropna` with the `how` and `thresh` parameters.

By default, `how='any'` (if you would like to check for yourself or see what other parameters the method has, run `example4.dropna?` in a code cell). You could alternatively specify `how='all'` so as to drop only rows or columns that contain all null values. Let's expand our example `DataFrame` to see this in action.

```python
example2[3] = np.nan
example2
```
|      |0  |1  |2  |3  |
|------|---|---|---|---|
|0     |1.0|NaN|7  |NaN|
|1     |2.0|5.0|8  |NaN|
|2     |NaN|6.0|9  |NaN|

The `thresh` parameter gives you finer-grained control: you set the number of *non-null* values that a row or column needs to have in order to be kept:
```python
example2.dropna(axis='rows', thresh=3)
```
```
	0	1	2	3
1	2.0	5.0	8	NaN
```
Here, the first and last row have been dropped, because they contain only two non-null values.

- **Filling null values**: Depending on your dataset, it can sometimes make more sense to fill null values with valid ones rather than drop them. You could use `isnull` to do this in place, but that can be laborious, particularly if you have a lot of values to fill. Because this is such a common task in data science, pandas provides `fillna`, which returns a copy of the `Series` or `DataFrame` with the missing values replaced with one of your choosing. Let's create another example `Series` to see how this works in practice.
```python
example3 = pd.Series([1, np.nan, 2, None, 3], index=list('abcde'))
example3
```
```
a    1.0
b    NaN
c    2.0
d    NaN
e    3.0
dtype: float64
```
You can fill all of the null entries with a single value, such as `0`:
```python
example3.fillna(0)
```
```
a    1.0
b    0.0
c    2.0
d    0.0
e    3.0
dtype: float64
```
You can **forward-fill** null values, which is to use the last valid value to fill a null:
```python
example3.fillna(method='ffill')
```
```
a    1.0
b    1.0
c    2.0
d    2.0
e    3.0
dtype: float64
```
You can also **back-fill** to propagate the next valid value backward to fill a null:
```python
example3.fillna(method='bfill')
```
```
a    1.0
b    2.0
c    2.0
d    3.0
e    3.0
dtype: float64
```
As you might guess, this works the same with `DataFrame`s, but you can also specify an `axis` along which to fill null values. taking the previously used `example2` again:
```python
example2.fillna(method='ffill', axis=1)
```
```
	0	1	2	3
0	1.0	1.0	7.0	7.0
1	2.0	5.0	8.0	8.0
2	NaN	6.0	9.0	9.0
```
Notice that when a previous value is not available for forward-filling, the null value remains.
> **मुख्य कुरा:** तपाईंको डेटासेटमा हराएका मानहरूलाई व्यवस्थापन गर्न धेरै तरिकाहरू छन्। तपाईंले प्रयोग गर्ने विशेष रणनीति (तिनीहरू हटाउने, प्रतिस्थापन गर्ने, वा कसरी प्रतिस्थापन गर्ने) उक्त डेटाको विशेषताहरूले निर्धारण गर्नुपर्छ। तपाईंले डेटासेटहरूलाई बढी ह्यान्डल र अन्तरक्रिया गर्दा हराएका मानहरूलाई कसरी व्यवस्थापन गर्ने भन्ने राम्रो ज्ञान विकास गर्नुहुनेछ।

## नक्कल डेटा हटाउने

> **शिक्षण लक्ष्य:** यस उपविभागको अन्त्यसम्ममा, तपाईंले DataFrames बाट नक्कल मानहरू पहिचान गर्न र हटाउन सहज महसुस गर्नुहुनेछ।

हराएको डेटाका अतिरिक्त, तपाईंले वास्तविक संसारका डेटासेटहरूमा प्रायः नक्कल गरिएको डेटा भेट्नुहुनेछ। सौभाग्यवश, `pandas` ले नक्कल प्रविष्टिहरू पत्ता लगाउन र हटाउन सजिलो माध्यम प्रदान गर्दछ।

- **नक्कल पहिचान गर्ने: `duplicated`**: तपाईंले `pandas` मा `duplicated` विधि प्रयोग गरेर सजिलै नक्कल मानहरू देख्न सक्नुहुन्छ, जसले `DataFrame` मा कुनै प्रविष्टि पहिलेको नक्कल हो कि होइन भन्ने संकेत गर्ने Boolean मास्क फर्काउँछ। यसलाई व्यवहारमा हेर्न अर्को उदाहरण `DataFrame` सिर्जना गरौं।
```python
example4 = pd.DataFrame({'letters': ['A','B'] * 2 + ['B'],
                         'numbers': [1, 2, 1, 3, 3]})
example4
```
|      |letters|numbers|
|------|-------|-------|
|0     |A      |1      |
|1     |B      |2      |
|2     |A      |1      |
|3     |B      |3      |
|4     |B      |3      |

```python
example4.duplicated()
```
```
0    False
1    False
2     True
3    False
4     True
dtype: bool
```
- **नक्कल हटाउने: `drop_duplicates`:** यसले `duplicated` मानहरू `False` भएका डेटा प्रतिलिपि फर्काउँछ:
```python
example4.drop_duplicates()
```
```
	letters	numbers
0	A	1
1	B	2
3	B	3
```
`duplicated` र `drop_duplicates` दुवैले सबै स्तम्भहरूलाई विचार गर्न डिफल्ट गर्छन् तर तपाईंले आफ्नो `DataFrame` मा केवल स्तम्भहरूको उपसमूह जाँच गर्न निर्दिष्ट गर्न सक्नुहुन्छ:
```python
example4.drop_duplicates(['letters'])
```
```
letters	numbers
0	A	1
1	B	2
```

> **मुख्य कुरा:** नक्कल डेटा हटाउनु लगभग प्रत्येक डेटा-विज्ञान परियोजनाको आवश्यक भाग हो। नक्कल डेटा तपाईंको विश्लेषणको नतिजा परिवर्तन गर्न सक्छ र तपाईंलाई गलत नतिजा दिन सक्छ!


## 🚀 चुनौती

सामग्रीहरू [Jupyter Notebook](https://github.com/microsoft/Data-Science-For-Beginners/blob/main/2-Working-With-Data/08-data-preparation/notebook.ipynb) को रूपमा उपलब्ध छन्। साथै, प्रत्येक खण्डपछि अभ्यासहरू छन्, तिनीहरूलाई प्रयास गर्नुहोस्!

## [पोस्ट-व्याख्यान क्विज](https://ff-quizzes.netlify.app/en/ds/)



## समीक्षा र आत्म-अध्ययन

तपाईंको डेटा विश्लेषण र मोडेलिङको लागि तयार पार्ने र सफा गर्ने धेरै तरिकाहरू पत्ता लगाउन र दृष्टिकोण गर्न सकिन्छ। डेटा सफा गर्ने महत्त्वपूर्ण चरण "हातको अनुभव" हो। Kaggle बाट यी चुनौतीहरू प्रयास गर्नुहोस् जसले यस पाठले समेटेको प्रविधिहरू अन्वेषण गर्न मद्दत गर्दछ।

- [डेटा सफा गर्ने चुनौती: मिति पार्सिङ](https://www.kaggle.com/rtatman/data-cleaning-challenge-parsing-dates/)

- [डेटा सफा गर्ने चुनौती: स्केल र सामान्यीकरण डेटा](https://www.kaggle.com/rtatman/data-cleaning-challenge-scale-and-normalize-data)


## असाइनमेन्ट

[फारमबाट डेटा मूल्याङ्कन गर्ने](assignment.md)

---

**अस्वीकरण**:  
यो दस्तावेज़ AI अनुवाद सेवा [Co-op Translator](https://github.com/Azure/co-op-translator) प्रयोग गरेर अनुवाद गरिएको छ। हामी शुद्धताको लागि प्रयास गर्छौं, तर कृपया ध्यान दिनुहोस् कि स्वचालित अनुवादमा त्रुटिहरू वा अशुद्धताहरू हुन सक्छ। यसको मूल भाषा मा रहेको मूल दस्तावेज़लाई आधिकारिक स्रोत मानिनुपर्छ। महत्वपूर्ण जानकारीको लागि, व्यावसायिक मानव अनुवाद सिफारिस गरिन्छ। यस अनुवादको प्रयोगबाट उत्पन्न हुने कुनै पनि गलतफहमी वा गलत व्याख्याको लागि हामी जिम्मेवार हुने छैनौं।