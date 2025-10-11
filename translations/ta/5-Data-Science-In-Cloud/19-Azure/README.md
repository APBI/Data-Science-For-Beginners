<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "472d3fab1c5be50f387336e7a686dbe1",
  "translation_date": "2025-10-11T15:30:38+00:00",
  "source_file": "5-Data-Science-In-Cloud/19-Azure/README.md",
  "language_code": "ta"
}
-->
# கிளவுடில் தரவியல் அறிவியல்: "Azure ML SDK" முறையில் 

|![ [(@sketchthedocs)](https://sketchthedocs.dev) உருவாக்கிய ஸ்கெட்ச் நோட் ](../../sketchnotes/19-DataScience-Cloud.png)|
|:---:|
| கிளவுடில் தரவியல் அறிவியல்: Azure ML SDK - _[@nitya](https://twitter.com/nitya) உருவாக்கிய ஸ்கெட்ச் நோட்_ |

உள்ளடக்க அட்டவணை:

- [கிளவுடில் தரவியல் அறிவியல்: "Azure ML SDK" முறையில்](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [முன்-பாடம் வினாடி வினா](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [1. அறிமுகம்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [1.1 Azure ML SDK என்றால் என்ன?](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [1.2 இதய செயலிழப்பு கணிப்பு திட்டம் மற்றும் தரவுத்தொகுப்பு அறிமுகம்](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [2. Azure ML SDK மூலம் ஒரு மாதிரியை பயிற்சி செய்யுதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.1 Azure ML வேலைப்பகுதியை உருவாக்குதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.2 கணிப்பொறி உதாரணத்தை உருவாக்குதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.3 தரவுத்தொகுப்பை ஏற்றுதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.4 நோட்புக்குகளை உருவாக்குதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.5 ஒரு மாதிரியை பயிற்சி செய்யுதல்](../../../../5-Data-Science-In-Cloud/19-Azure)
      - [2.5.1 வேலைப்பகுதி, பரிசோதனை, கணிப்பொறி கிளஸ்டர் மற்றும் தரவுத்தொகுப்பை அமைத்தல்](../../../../5-Data-Science-In-Cloud/19-Azure)
      - [2.5.2 AutoML கட்டமைப்பு மற்றும் பயிற்சி](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [3. Azure ML SDK மூலம் மாதிரி பிரசாரம் மற்றும் இறுதிப்புள்ளி பயன்பாடு](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.1 சிறந்த மாதிரியை சேமித்தல்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.2 மாதிரி பிரசாரம்](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.3 இறுதிப்புள்ளி பயன்பாடு](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [🚀 சவால்](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [பாடத்திற்குப் பிந்தைய வினாடி வினா](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [மறுபரிசீலனை மற்றும் சுயபயிற்சி](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [வினாத்தாள்](../../../../5-Data-Science-In-Cloud/19-Azure)

## [முன்-பாடம் வினாடி வினா](https://ff-quizzes.netlify.app/en/ds/quiz/36)

## 1. அறிமுகம்

### 1.1 Azure ML SDK என்றால் என்ன?

தரவியல் அறிஞர்கள் மற்றும் AI டெவலப்பர்கள் Azure Machine Learning SDK-ஐப் பயன்படுத்தி Azure Machine Learning சேவையுடன் இயங்கும் இயந்திரக் கற்றல் பணிகளை உருவாக்கி இயக்குகிறார்கள். Python சூழலில், Jupyter Notebooks, Visual Studio Code அல்லது உங்களுக்கு பிடித்த Python IDE போன்றவற்றில் இந்த சேவையுடன் தொடர்பு கொள்ளலாம்.

SDK-யின் முக்கிய பகுதிகள்:

- இயந்திரக் கற்றல் பரிசோதனைகளில் பயன்படுத்தப்படும் தரவுத்தொகுப்புகளை ஆராய்ந்து, தயாரித்து, அவற்றின் ஆயுள்நிலையை நிர்வகிக்கவும்.
- உங்கள் இயந்திரக் கற்றல் பரிசோதனைகளை கண்காணிக்க, பதிவு செய்ய மற்றும் ஒழுங்கமைக்க கிளவுட் வளங்களை நிர்வகிக்கவும்.
- மாதிரிகளை உள்ளூர் அல்லது GPU-ஐ ஆதரிக்கும் கிளவுட் வளங்களைப் பயன்படுத்தி பயிற்சி செய்யவும்.
- தானியங்கி இயந்திரக் கற்றலைப் பயன்படுத்தவும், இது கட்டமைப்பு அளவுருக்களையும் பயிற்சி தரவையும் ஏற்கிறது. இது ஆல்காரிதம்கள் மற்றும் ஹைப்பர்பாராமீட்டர் அமைப்புகளைத் தேர்ந்தெடுத்து கணிப்புகளுக்கு சிறந்த மாதிரியை கண்டறிய முயற்சிக்கிறது.
- பயிற்சி செய்யப்பட்ட மாதிரிகளை RESTful சேவைகளாக மாற்றி, எந்த பயன்பாட்டிலும் பயன்படுத்தக்கூடிய வலை சேவைகளைப் பிரசாரம் செய்யவும்.

[Azure Machine Learning SDK பற்றி மேலும் அறிக](https://docs.microsoft.com/python/api/overview/azure/ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109)

[முந்தைய பாடத்தில்](../18-Low-Code/README.md), குறைந்த குறியீடு/குறியீடு இல்லாத முறையில் மாதிரியை பயிற்சி செய்ய, பிரசாரம் செய்ய மற்றும் பயன்படுத்துவது எப்படி என்பதைப் பார்த்தோம். இதய செயலிழப்பு தரவுத்தொகுப்பைப் பயன்படுத்தி இதய செயலிழப்பு கணிப்பு மாதிரியை உருவாக்கினோம். இந்த பாடத்தில், அதே செயல்முறையை Azure Machine Learning SDK-ஐப் பயன்படுத்தி செய்வோம்.

![திட்டம் வரைபடம்](../../../../translated_images/project-schema.420e56d495624541eaecf2b737f138c86fb7d8162bb1c0bf8783c350872ffc4d.ta.png)

### 1.2 இதய செயலிழப்பு கணிப்பு திட்டம் மற்றும் தரவுத்தொகுப்பு அறிமுகம்

இதய செயலிழப்பு கணிப்பு திட்டம் மற்றும் தரவுத்தொகுப்பு அறிமுகத்திற்காக [இங்கே](../18-Low-Code/README.md) பார்க்கவும்.

## 2. Azure ML SDK மூலம் ஒரு மாதிரியை பயிற்சி செய்யுதல்

### 2.1 Azure ML வேலைப்பகுதியை உருவாக்குதல்

எளிமைப்படுத்த, நாம் Jupyter Notebook-ல் வேலை செய்வோம். இதற்காக, உங்களிடம் ஏற்கனவே ஒரு வேலைப்பகுதி மற்றும் கணிப்பொறி உதாரணம் இருக்க வேண்டும். உங்களிடம் ஏற்கனவே வேலைப்பகுதி இருந்தால், நேரடியாக 2.3 நோட்புக் உருவாக்கம் பிரிவுக்கு செல்லலாம்.

இல்லையெனில், [முந்தைய பாடத்தில்](../18-Low-Code/README.md) உள்ள **2.1 Azure ML வேலைப்பகுதியை உருவாக்குதல்** பிரிவின் வழிமுறைகளைப் பின்பற்றவும்.

### 2.2 கணிப்பொறி உதாரணத்தை உருவாக்குதல்

நாம் முன்பு உருவாக்கிய [Azure ML வேலைப்பகுதியில்](https://ml.azure.com/), கணிப்பொறி மெனுவுக்கு சென்று கிடைக்கும் கணிப்பொறி வளங்களைப் பாருங்கள்.

![கணிப்பொறி உதாரணம் 1](../../../../translated_images/compute-instance-1.dba347cb199ca4996b3e3d649295ed95626ba481479d3986557b9b98e76d8816.ta.png)

Jupyter Notebook-ஐ வழங்க ஒரு கணிப்பொறி உதாரணத்தை உருவாக்குவோம். 
1. + New பொத்தானை அழுத்தவும். 
2. உங்கள் கணிப்பொறி உதாரணத்திற்கு ஒரு பெயரை கொடுங்கள்.
3. உங்கள் விருப்பங்களைத் தேர்ந்தெடுக்கவும்: CPU அல்லது GPU, VM அளவு மற்றும் மைய எண்ணிக்கை.
4. Create பொத்தானை அழுத்தவும்.

வாழ்த்துக்கள், நீங்கள் ஒரு கணிப்பொறி உதாரணத்தை வெற்றிகரமாக உருவாக்கிவிட்டீர்கள்! [நோட்புக் உருவாக்கம்](../../../../5-Data-Science-In-Cloud/19-Azure) பிரிவில் இந்த கணிப்பொறி உதாரணத்தைப் பயன்படுத்துவோம்.

### 2.3 தரவுத்தொகுப்பை ஏற்றுதல்

இன்னும் தரவுத்தொகுப்பை ஏற்றவில்லை என்றால், [முந்தைய பாடத்தில்](../18-Low-Code/README.md) உள்ள **2.3 தரவுத்தொகுப்பை ஏற்றுதல்** பிரிவை பார்க்கவும்.

### 2.4 நோட்புக்குகளை உருவாக்குதல்

> **_குறிப்பு:_** அடுத்த படிக்காக, நீங்கள் புதிய நோட்புக் ஒன்றை உருவாக்கலாம் அல்லது [நாம் உருவாக்கிய நோட்புக்கை](notebook.ipynb) உங்கள் Azure ML ஸ்டுடியோவில் பதிவேற்றலாம். பதிவேற்ற, "Notebook" மெனுவை கிளிக் செய்து நோட்புக்கை பதிவேற்றவும்.

நோட்புக்குகள் தரவியல் அறிவியல் செயல்முறையின் முக்கியமான பகுதியாகும். அவை தரவுகளை ஆராய, கணிப்பொறி கிளஸ்டரை அழைக்க மாதிரியை பயிற்சி செய்ய, அல்லது இறுதிப்புள்ளி பிரசாரத்திற்கு அழைக்க பயன்படுத்தப்படுகின்றன.

நோட்புக் உருவாக்க, Jupyter Notebook உதாரணத்தை வழங்கும் கணிப்பொறி நொடுக்கு தேவை. மீண்டும் [Azure ML வேலைப்பகுதிக்கு](https://ml.azure.com/) சென்று கணிப்பொறி உதாரணங்களை கிளிக் செய்யவும். நீங்கள் [முன்பு உருவாக்கிய கணிப்பொறி உதாரணத்தை](../../../../5-Data-Science-In-Cloud/19-Azure) காணலாம்.

1. Applications பிரிவில், Jupyter விருப்பத்தை கிளிக் செய்யவும். 
2. "Yes, I understand" பெட்டியை அடையாளமிடி மற்றும் Continue பொத்தானை அழுத்தவும்.
![நோட்புக் 1](../../../../translated_images/notebook-1.12998af7b02c83f536c11b3aeba561be16e0f05e94146600728ec64270ce1105.ta.png)
3. இது உங்கள் Jupyter Notebook உதாரணத்துடன் புதிய உலாவி தாவலைத் திறக்கும். "New" பொத்தானை அழுத்தி ஒரு நோட்புக் உருவாக்கவும்.

![நோட்புக் 2](../../../../translated_images/notebook-2.9a657c037e34f1cf26c0212f5ee9e2da8545b3e107c7682c55114e494167a8aa.ta.png)

இப்போது, நமக்கு ஒரு நோட்புக் உள்ளது. Azure ML SDK-யுடன் மாதிரியை பயிற்சி செய்ய தொடங்கலாம்.

### 2.5 ஒரு மாதிரியை பயிற்சி செய்யுதல்

முதலில், சந்தேகம் இருந்தால், [Azure ML SDK ஆவணங்களை](https://docs.microsoft.com/python/api/overview/azure/ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) பார்க்கவும். இந்த பாடத்தில் நாம் காணும் தொகுதிகளைப் புரிந்துகொள்ள தேவையான அனைத்து தகவல்களும் இதில் உள்ளன.

#### 2.5.1 வேலைப்பகுதி, பரிசோதனை, கணிப்பொறி கிளஸ்டர் மற்றும் தரவுத்தொகுப்பை அமைத்தல்

`workspace`-ஐ கட்டமைப்பு கோப்பிலிருந்து கீழே உள்ள குறியீட்டை பயன்படுத்தி ஏற்ற வேண்டும்:

```python
from azureml.core import Workspace
ws = Workspace.from_config()
```

இது `Workspace` வகையைச் சேர்ந்த ஒரு பொருளை திருப்பும், இது வேலைப்பகுதியை பிரதிநிதித்துவப்படுத்தும். பின்னர், நீங்கள் கீழே உள்ள குறியீட்டை பயன்படுத்தி ஒரு `experiment` உருவாக்க வேண்டும்:

```python
from azureml.core import Experiment
experiment_name = 'aml-experiment'
experiment = Experiment(ws, experiment_name)
```

வேலைப்பகுதியிலிருந்து ஒரு பரிசோதனையை பெற அல்லது உருவாக்க, நீங்கள் பரிசோதனையை அதன் பெயரைப் பயன்படுத்தி கோர வேண்டும். பரிசோதனை பெயர் 3-36 எழுத்துகளுக்கு இடையில் இருக்க வேண்டும், ஒரு எழுத்து அல்லது எண்ணுடன் தொடங்க வேண்டும், மற்றும் எழுத்துக்கள், எண்கள், அடிக்கோடுகள் மற்றும் கோடுகள் மட்டுமே கொண்டிருக்க வேண்டும். வேலைப்பகுதியில் பரிசோதனை கிடைக்காவிட்டால், புதிய பரிசோதனை உருவாக்கப்படும்.

இப்போது, பயிற்சிக்காக ஒரு கணிப்பொறி கிளஸ்டரை உருவாக்க வேண்டும். இந்த படி சில நிமிடங்கள் ஆகும்:

```python
from azureml.core.compute import AmlCompute

aml_name = "heart-f-cluster"
try:
    aml_compute = AmlCompute(ws, aml_name)
    print('Found existing AML compute context.')
except:
    print('Creating new AML compute context.')
    aml_config = AmlCompute.provisioning_configuration(vm_size = "Standard_D2_v2", min_nodes=1, max_nodes=3)
    aml_compute = AmlCompute.create(ws, name = aml_name, provisioning_configuration = aml_config)
    aml_compute.wait_for_completion(show_output = True)

cts = ws.compute_targets
compute_target = cts[aml_name]
```

தரவுத்தொகுப்பை வேலைப்பகுதியிலிருந்து தரவுத்தொகுப்பு பெயரைப் பயன்படுத்தி பெறலாம்:

```python
dataset = ws.datasets['heart-failure-records']
df = dataset.to_pandas_dataframe()
df.describe()
```


#### 2.5.2 AutoML கட்டமைப்பு மற்றும் பயிற்சி

AutoML கட்டமைப்பை அமைக்க, [AutoMLConfig வகுப்பைப்](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.automlconfig(class)?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) பயன்படுத்தவும்.

ஆவணத்தில் விவரிக்கப்பட்டுள்ளபடி, நீங்கள் பல அளவுருக்களுடன் விளையாடலாம். இந்த திட்டத்திற்காக, நாம் பின்வரும் அளவுருக்களைப் பயன்படுத்துவோம்:

- `experiment_timeout_minutes`: பரிசோதனை இயங்க அனுமதிக்கப்பட்ட அதிகபட்ச நேரம் (நிமிடங்களில்).
- `max_concurrent_iterations`: பரிசோதனைக்கு அனுமதிக்கப்பட்ட அதிகபட்ச ஒரே நேர பயிற்சி மீள்பார்வைகள்.
- `primary_metric`: பரிசோதனையின் நிலையை தீர்மானிக்க பயன்படுத்தப்படும் முதன்மை அளவுகோல்.
- `compute_target`: Automated Machine Learning பரிசோதனையை இயக்க Azure Machine Learning கணிப்பொறி இலக்கு.
- `task`: இயக்க வேண்டிய பணியின் வகை. 'classification', 'regression', அல்லது 'forecasting' ஆகியவை மதிப்புகளாக இருக்கலாம்.
- `training_data`: பரிசோதனையில் பயன்படுத்தப்படும் பயிற்சி தரவுகள். இது பயிற்சி அம்சங்களையும் ஒரு லேபிள் நெடுவரிசையையும் கொண்டிருக்க வேண்டும்.
- `label_column_name`: லேபிள் நெடுவரிசையின் பெயர்.
- `path`: Azure Machine Learning திட்ட கோப்புறையின் முழு பாதை.
- `enable_early_stopping`: குறுகிய காலத்தில் மதிப்பெண் மேம்படவில்லை என்றால், முன்கூட்டியே நிறுத்தலை இயக்க வேண்டுமா என்பதைத் தீர்மானிக்கிறது.
- `featurization`: தானாக அம்சமயமாக்கல் படியைச் செய்ய வேண்டுமா அல்லது தனிப்பயன் அம்சமயமாக்கலைப் பயன்படுத்த வேண்டுமா என்பதைத் தீர்மானிக்கிறது.
- `debug_log`: பிழைதிருத்த தகவல்களை எழுதுவதற்கான பதிவு கோப்பு.

```python
from azureml.train.automl import AutoMLConfig

project_folder = './aml-project'

automl_settings = {
    "experiment_timeout_minutes": 20,
    "max_concurrent_iterations": 3,
    "primary_metric" : 'AUC_weighted'
}

automl_config = AutoMLConfig(compute_target=compute_target,
                             task = "classification",
                             training_data=dataset,
                             label_column_name="DEATH_EVENT",
                             path = project_folder,  
                             enable_early_stopping= True,
                             featurization= 'auto',
                             debug_log = "automl_errors.log",
                             **automl_settings
                            )
```

இப்போது உங்கள் கட்டமைப்பு அமைக்கப்பட்டுள்ளதால், கீழே உள்ள குறியீட்டை பயன்படுத்தி மாதிரியை பயிற்சி செய்யலாம். இந்த படி உங்கள் கிளஸ்டர் அளவைப் பொறுத்து ஒரு மணி நேரம் வரை ஆகலாம்.

```python
remote_run = experiment.submit(automl_config)
```

பரிசோதனைகளை காண RunDetails விட்ஜெட்டை இயக்கலாம்.
```python
from azureml.widgets import RunDetails
RunDetails(remote_run).show()
```


## 3. Azure ML SDK மூலம் மாதிரி பிரசாரம் மற்றும் இறுதிப்புள்ளி பயன்பாடு

### 3.1 சிறந்த மாதிரியை சேமித்தல்

`remote_run` என்பது [AutoMLRun](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.run.automlrun?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) வகையைச் சேர்ந்த ஒரு பொருள். இந்த பொருளில் `get_output()` என்ற முறை உள்ளது, இது சிறந்த இயக்கத்தையும் அதற்கான பொருத்தமான மாதிரியையும் திருப்பும்.

```python
best_run, fitted_model = remote_run.get_output()
```

சிறந்த மாதிரிக்கான அளவுருக்களை காண, `fitted_model`-ஐ அச்சிட்டு, சிறந்த மாதிரியின் பண்புகளை [get_properties()](https://docs.microsoft.com/python/api/azureml-core/azureml.core.run(class)?view=azure-ml-py#azureml_core_Run_get_properties?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) முறையைப் பயன்படுத்தி பார்க்கலாம்.

```python
best_run.get_properties()
```

இப்போது [register_model](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.run.automlrun?view=azure-ml-py#register-model-model-name-none--description-none--tags-none--iteration-none--metric-none-?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) முறையைப் பயன்படுத்தி மாதிரியை பதிவு செய்யவும்.
```python
model_name = best_run.properties['model_name']
script_file_name = 'inference/score.py'
best_run.download_file('outputs/scoring_file_v_1_0_0.py', 'inference/score.py')
description = "aml heart failure project sdk"
model = best_run.register_model(model_name = model_name,
                                model_path = './outputs/',
                                description = description,
                                tags = None)
```


### 3.2 மாதிரி பிரசாரம்

சிறந்த மாதிரி சேமிக்கப்பட்ட பிறகு, [InferenceConfig](https://docs.microsoft.com/python/api/azureml-core/azureml.core.model.inferenceconfig?view=azure-ml-py?ocid=AID3041109) வகுப்பைப் பயன்படுத்தி அதை பிரசாரம் செய்யலாம். InferenceConfig என்பது பிரசாரத்திற்கான தனிப்பயன் சூழலுக்கான கட்டமைப்பு அமைப்புகளை பிரதிநிதித்துவப்படுத்துகிறது. [AciWebservice](https://docs.microsoft.com/python/api/azureml-core/azureml.core.webservice.aciwebservice?view=azure-ml-py) வகுப்பு Azure Container Instances-ல் ஒரு வலை சேவையாக பிரசாரம் செய்யப்பட்ட இயந்திரக் கற்றல் மாதிரியை பிரதிநிதித்துவப்படுத்துகிறது. பிரசாரம் செய்யப்பட்ட சேவை ஒரு மாடல், ஸ்கிரிப்ட் மற்றும் தொடர்புடைய கோப்புகளிலிருந்து உருவாக்கப்படுகிறது. முடிவில் கிடைக்கும் வலை சேவை ஒரு சுமை-மீட்டப்பட்ட, HTTP இறுதிப்புள்ளி கொண்ட REST API ஆகும். இந்த API-க்கு தரவுகளை அனுப்பி, மாதிரி திருப்பும் கணிப்பை பெறலாம்.

மாதிரி [deploy](https://docs.microsoft.com/python/api/azureml-core/azureml.core.model(class)?view=azure-ml-py#deploy-workspace--name--models--inference-config-none--deployment-config-none--deployment-target-none--overwrite-false--show-output-false-?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) முறையைப் பயன்படுத்தி பிரசாரம் செய்யப்படுகிறது.

```python
from azureml.core.model import InferenceConfig, Model
from azureml.core.webservice import AciWebservice

inference_config = InferenceConfig(entry_script=script_file_name, environment=best_run.get_environment())

aciconfig = AciWebservice.deploy_configuration(cpu_cores = 1,
                                               memory_gb = 1,
                                               tags = {'type': "automl-heart-failure-prediction"},
                                               description = 'Sample service for AutoML Heart Failure Prediction')

aci_service_name = 'automl-hf-sdk'
aci_service = Model.deploy(ws, aci_service_name, [model], inference_config, aciconfig)
aci_service.wait_for_deployment(True)
print(aci_service.state)
```

இந்த படி சில நிம
```python
data = {
    "data":
    [
        {
            'age': "60",
            'anaemia': "false",
            'creatinine_phosphokinase': "500",
            'diabetes': "false",
            'ejection_fraction': "38",
            'high_blood_pressure': "false",
            'platelets': "260000",
            'serum_creatinine': "1.40",
            'serum_sodium': "137",
            'sex': "false",
            'smoking': "false",
            'time': "130",
        },
    ],
}

test_sample = str.encode(json.dumps(data))
```
 பின்னர் நீங்கள் இந்த உள்ளீட்டை உங்கள் மாதிரிக்கு கணிப்பு செய்ய அனுப்பலாம்:

```python
response = aci_service.run(input_data=test_sample)
response
```
 இதன் வெளியீடு `'{"result": [false]}'` ஆக இருக்கும். இதன் பொருள், நாம் endpoint-க்கு அனுப்பிய நோயாளியின் உள்ளீடு `false` எனும் கணிப்பை உருவாக்கியது, இது இந்த நபர் இதயக் கோளாறு ஏற்படும் வாய்ப்பு இல்லை என்பதைக் குறிக்கிறது.

வாழ்த்துக்கள்! நீங்கள் Azure ML SDK-யை பயன்படுத்தி Azure ML-ல் பயிற்சி செய்து வெளியிட்ட மாதிரியை பயன்படுத்த முடிந்தது!

> **_NOTE:_** திட்டத்தை முடித்தவுடன், அனைத்து வளங்களையும் நீக்க மறக்காதீர்கள்.

## 🚀 சவால்

SDK மூலம் நீங்கள் செய்யக்கூடிய பல விஷயங்கள் உள்ளன, ஆனால் இந்த பாடத்தில் அவற்றை அனைத்தையும் பார்க்க முடியாது. ஆனால் நல்ல செய்தி என்னவென்றால், SDK ஆவணங்களை எளிதாகப் புரிந்துகொள்வது உங்களை நீண்ட தூரம் முன்னேற்றும். Azure ML SDK ஆவணங்களைப் பாருங்கள் மற்றும் `Pipeline` வகுப்பைத் தேடுங்கள், இது பைப்ப்லைன்களை உருவாக்க அனுமதிக்கிறது. பைப்ப்லைன் என்பது ஒரு வேலைப்பாடாக செயல்படுத்தக்கூடிய படிகள் தொகுப்பாகும்.

**HINT:** [SDK ஆவணங்கள்](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) பக்கம் சென்று தேடுபொறியில் "Pipeline" போன்ற முக்கிய வார்த்தைகளைத் தேடுங்கள். தேடல் முடிவுகளில் `azureml.pipeline.core.Pipeline` வகுப்பு இருக்க வேண்டும்.

## [பாடத்திற்குப் பிந்தைய வினாடி வினா](https://ff-quizzes.netlify.app/en/ds/quiz/37)

## மதிப்பீடு & சுயபடிப்பு

இந்த பாடத்தில், நீங்கள் Azure ML SDK-யை பயன்படுத்தி மேகத்தில் இதய கோளாறு அபாயத்தை கணிக்க ஒரு மாதிரியை பயிற்சி, வெளியீடு மற்றும் பயன்படுத்துவது எப்படி என்பதை கற்றுக்கொண்டீர்கள். Azure ML SDK பற்றிய கூடுதல் தகவலுக்கு இந்த [ஆவணத்தை](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) பாருங்கள். Azure ML SDK-யை பயன்படுத்தி உங்கள் சொந்த மாதிரியை உருவாக்க முயற்சிக்கவும்.

## பணிக்கட்டளை

[Azure ML SDK-யை பயன்படுத்தி தரவியல் அறிவியல் திட்டம்](assignment.md)

---

**குறிப்பு**:  
இந்த ஆவணம் [Co-op Translator](https://github.com/Azure/co-op-translator) என்ற AI மொழிபெயர்ப்பு சேவையைப் பயன்படுத்தி மொழிபெயர்க்கப்பட்டுள்ளது. எங்கள் தரச்செயல்முறைகளுக்கு முக்கியத்துவம் அளிக்கின்றோம், ஆனால் தானியக்க மொழிபெயர்ப்புகளில் பிழைகள் அல்லது தவறான தகவல்கள் இருக்கக்கூடும் என்பதை தயவுசெய்து கவனத்தில் கொள்ளவும். அதன் இயல்பான மொழியில் உள்ள மூல ஆவணம் அதிகாரப்பூர்வ ஆதாரமாக கருதப்பட வேண்டும். முக்கியமான தகவல்களுக்கு, தொழில்முறை மனித மொழிபெயர்ப்பு பரிந்துரைக்கப்படுகிறது. இந்த மொழிபெயர்ப்பைப் பயன்படுத்துவதால் ஏற்படும் எந்த தவறான புரிதல்கள் அல்லது தவறான விளக்கங்களுக்கு நாங்கள் பொறுப்பல்ல.