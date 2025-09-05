<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "5da2d6b3736f6d668b89de9bf3bdd31b",
  "translation_date": "2025-09-05T06:10:05+00:00",
  "source_file": "5-Data-Science-In-Cloud/19-Azure/README.md",
  "language_code": "sr"
}
-->
# Наука о подацима у облаку: Путем "Azure ML SDK"

|![ Скетч од [(@sketchthedocs)](https://sketchthedocs.dev) ](../../sketchnotes/19-DataScience-Cloud.png)|
|:---:|
| Наука о подацима у облаку: Azure ML SDK - _Скетч од [@nitya](https://twitter.com/nitya)_ |

Садржај:

- [Наука о подацима у облаку: Путем "Azure ML SDK"](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [Квиз пре предавања](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [1. Увод](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [1.1 Шта је Azure ML SDK?](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [1.2 Пројекат предвиђања срчане инсуфицијенције и увод у скуп података](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [2. Тренирање модела са Azure ML SDK](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.1 Креирање Azure ML радног простора](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.2 Креирање рачунарског инстанца](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.3 Учитавање скупа података](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.4 Креирање бележница](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [2.5 Тренирање модела](../../../../5-Data-Science-In-Cloud/19-Azure)
      - [2.5.1 Подешавање радног простора, експеримента, рачунарског кластера и скупа података](../../../../5-Data-Science-In-Cloud/19-Azure)
      - [2.5.2 Конфигурација AutoML и тренирање](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [3. Деплојмент модела и коришћење ендпоинта са Azure ML SDK](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.1 Чување најбољег модела](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.2 Деплојмент модела](../../../../5-Data-Science-In-Cloud/19-Azure)
    - [3.3 Коришћење ендпоинта](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [🚀 Изазов](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [Квиз након предавања](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [Преглед и самостално учење](../../../../5-Data-Science-In-Cloud/19-Azure)
  - [Задатак](../../../../5-Data-Science-In-Cloud/19-Azure)

## [Квиз пре предавања](https://purple-hill-04aebfb03.1.azurestaticapps.net/quiz/36)

## 1. Увод

### 1.1 Шта је Azure ML SDK?

Научници за податке и развојни инжењери за вештачку интелигенцију користе Azure Machine Learning SDK за креирање и извршавање радних токова машинског учења уз помоћ Azure Machine Learning услуге. Можете комуницирати са услугом у било ком Python окружењу, укључујући Jupyter бележнице, Visual Studio Code или ваш омиљени Python IDE.

Кључне области SDK-а укључују:

- Истраживање, припрему и управљање животним циклусом скупова података који се користе у експериментима машинског учења.
- Управљање ресурсима у облаку за праћење, бележење и организовање ваших експеримената машинског учења.
- Тренирање модела локално или коришћењем ресурса у облаку, укључујући тренирање модела убрзано GPU-ом.
- Коришћење аутоматизованог машинског учења, које прихвата параметре конфигурације и податке за тренирање. Аутоматски пролази кроз алгоритме и подешавања хиперпараметара како би пронашао најбољи модел за предвиђања.
- Деплојмент веб услуга за претварање ваших тренираних модела у RESTful услуге које се могу користити у било којој апликацији.

[Сазнајте више о Azure Machine Learning SDK](https://docs.microsoft.com/python/api/overview/azure/ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109)

У [претходној лекцији](../18-Low-Code/README.md), видели смо како да тренирамо, деплојујемо и користимо модел на начин са мало или без кода. Користили смо скуп података о срчаној инсуфицијенцији за генерисање модела за предвиђање срчане инсуфицијенције. У овој лекцији ћемо урадити исту ствар, али користећи Azure Machine Learning SDK.

![шема-пројекта](../../../../5-Data-Science-In-Cloud/19-Azure/images/project-schema.PNG)

### 1.2 Пројекат предвиђања срчане инсуфицијенције и увод у скуп података

Погледајте [овде](../18-Low-Code/README.md) увод у пројекат предвиђања срчане инсуфицијенције и скуп података.

## 2. Тренирање модела са Azure ML SDK

### 2.1 Креирање Azure ML радног простора

Ради једноставности, радићемо у Jupyter бележници. Ово подразумева да већ имате радни простор и рачунарски инстанц. Ако већ имате радни простор, можете директно прећи на одељак 2.3 Креирање бележнице.

Ако не, пратите упутства у одељку **2.1 Креирање Azure ML радног простора** у [претходној лекцији](../18-Low-Code/README.md) да бисте креирали радни простор.

### 2.2 Креирање рачунарског инстанца

У [Azure ML радном простору](https://ml.azure.com/) који смо раније креирали, идите у мени за рачунарске ресурсе и видећете различите доступне рачунарске ресурсе.

![рачунарски-инстанц-1](../../../../5-Data-Science-In-Cloud/19-Azure/images/compute-instance-1.PNG)

Хајде да креирамо рачунарски инстанц за постављање Jupyter бележнице.  
1. Кликните на дугме + New.  
2. Дајте име вашем рачунарском инстанцу.  
3. Изаберите опције: CPU или GPU, величину VM-а и број језгара.  
4. Кликните на дугме Create.  

Честитамо, управо сте креирали рачунарски инстанц! Користићемо овај инстанц за креирање бележнице у одељку [Креирање бележница](../../../../5-Data-Science-In-Cloud/19-Azure).

### 2.3 Учитавање скупа података

Погледајте [претходну лекцију](../18-Low-Code/README.md) у одељку **2.3 Учитавање скупа података** ако још нисте отпремили скуп података.

### 2.4 Креирање бележница

> **_НАПОМЕНА:_** За следећи корак можете или креирати нову бележницу од почетка, или можете отпремити [бележницу коју смо креирали](../../../../5-Data-Science-In-Cloud/19-Azure/notebook.ipynb) у вашем Azure ML студију. Да бисте је отпремили, једноставно кликните на мени "Notebook" и отпремите бележницу.

Бележнице су веома важан део процеса науке о подацима. Могу се користити за спровођење истраживачке анализе података (EDA), позивање на рачунарски кластер за тренирање модела, као и на кластер за инференцију ради деплојмента ендпоинта.

Да бисмо креирали бележницу, потребан нам је рачунарски чвор који покреће инстанцу Jupyter бележнице. Вратите се у [Azure ML радни простор](https://ml.azure.com/) и кликните на Compute instances. У листи рачунарских инстанци требало би да видите [рачунарски инстанц који смо раније креирали](../../../../5-Data-Science-In-Cloud/19-Azure).

1. У одељку Applications, кликните на опцију Jupyter.  
2. Означите поље "Yes, I understand" и кликните на дугме Continue.  
![бележница-1](../../../../5-Data-Science-In-Cloud/19-Azure/images/notebook-1.PNG)  
3. Ово би требало да отвори нову картицу у прегледачу са вашом инстанцом Jupyter бележнице. Кликните на дугме "New" да бисте креирали бележницу.  

![бележница-2](../../../../5-Data-Science-In-Cloud/19-Azure/images/notebook-2.PNG)

Сада када имамо бележницу, можемо започети тренирање модела са Azure ML SDK.

### 2.5 Тренирање модела

Прво, ако икада имате недоумицу, погледајте [документацију Azure ML SDK](https://docs.microsoft.com/python/api/overview/azure/ml?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109). Она садржи све потребне информације за разумевање модула које ћемо видети у овој лекцији.

#### 2.5.1 Подешавање радног простора, експеримента, рачунарског кластера и скупа података

Потребно је да учитате `workspace` из конфигурационе датотеке користећи следећи код:

```python
from azureml.core import Workspace
ws = Workspace.from_config()
```

Ово враћа објекат типа `Workspace` који представља радни простор. Затим је потребно креирати `experiment` користећи следећи код:

```python
from azureml.core import Experiment
experiment_name = 'aml-experiment'
experiment = Experiment(ws, experiment_name)
```

Да бисте добили или креирали експеримент из радног простора, захтевате експеримент користећи његово име. Име експеримента мора имати 3-36 карактера, почети словом или бројем и може садржати само слова, бројеве, подвлаке и цртице. Ако експеримент није пронађен у радном простору, креира се нови.

Сада је потребно креирати рачунарски кластер за тренирање користећи следећи код. Имајте на уму да овај корак може трајати неколико минута.

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

Можете добити скуп података из радног простора користећи име скупа података на следећи начин:

```python
dataset = ws.datasets['heart-failure-records']
df = dataset.to_pandas_dataframe()
df.describe()
```

#### 2.5.2 Конфигурација AutoML и тренирање

Да бисте подесили конфигурацију AutoML, користите [AutoMLConfig класу](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.automlconfig(class)?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109).

Као што је описано у документацији, постоји много параметара са којима можете експериментисати. За овај пројекат, користићемо следеће параметре:

- `experiment_timeout_minutes`: Максимално време (у минутима) које је експерименту дозвољено да траје пре него што се аутоматски заустави и резултати постану доступни.
- `max_concurrent_iterations`: Максималан број истовремених итерација тренирања дозвољених за експеримент.
- `primary_metric`: Примарна метрика која се користи за одређивање статуса експеримента.
- `compute_target`: Azure Machine Learning рачунарска мета на којој се извршава експеримент аутоматизованог машинског учења.
- `task`: Тип задатка који се извршава. Вредности могу бити 'classification', 'regression' или 'forecasting' у зависности од типа проблема аутоматизованог машинског учења.
- `training_data`: Скуп података за тренирање који се користи унутар експеримента. Требало би да садржи и карактеристике за тренирање и колону са ознакама (опционално и колону са тежинама узорака).
- `label_column_name`: Назив колоне са ознакама.
- `path`: Пуни пут до фасцикле Azure Machine Learning пројекта.
- `enable_early_stopping`: Да ли је омогућено рано заустављање ако се резултати не побољшавају у кратком року.
- `featurization`: Индикатор да ли би корак феатуризације требало аутоматски извршити или не, или да ли би требало користити прилагођена феатуризација.
- `debug_log`: Лог датотека у коју се уписују информације за отклањање грешака.

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

Сада када сте подесили конфигурацију, можете тренирати модел користећи следећи код. Овај корак може трајати до сат времена у зависности од величине вашег кластера.

```python
remote_run = experiment.submit(automl_config)
```

Можете покренути RunDetails виџет да бисте приказали различите експерименте.

```python
from azureml.widgets import RunDetails
RunDetails(remote_run).show()
```

## 3. Деплојмент модела и коришћење ендпоинта са Azure ML SDK

### 3.1 Чување најбољег модела

`remote_run` је објекат типа [AutoMLRun](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.run.automlrun?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109). Овај објекат садржи метод `get_output()` који враћа најбољу итерацију и одговарајући обучени модел.

```python
best_run, fitted_model = remote_run.get_output()
```

Можете видети параметре коришћене за најбољи модел тако што ћете једноставно исписати `fitted_model` и видети својства најбољег модела коришћењем методе [get_properties()](https://docs.microsoft.com/python/api/azureml-core/azureml.core.run(class)?view=azure-ml-py#azureml_core_Run_get_properties?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109).

```python
best_run.get_properties()
```

Сада региструјте модел помоћу методе [register_model](https://docs.microsoft.com/python/api/azureml-train-automl-client/azureml.train.automl.run.automlrun?view=azure-ml-py#register-model-model-name-none--description-none--tags-none--iteration-none--metric-none-?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109).

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

### 3.2 Деплојмент модела

Када је најбољи модел сачуван, можемо га деплојовати помоћу класе [InferenceConfig](https://docs.microsoft.com/python/api/azureml-core/azureml.core.model.inferenceconfig?view=azure-ml-py?ocid=AID3041109). InferenceConfig представља конфигурационе поставке за прилагођено окружење које се користи за деплојмент. Класа [AciWebservice](https://docs.microsoft.com/python/api/azureml-core/azureml.core.webservice.aciwebservice?view=azure-ml-py) представља модел машинског учења деплојован као веб услуга на Azure Container Instances. Деплојована услуга је балансирани HTTP ендпоинт са REST API-јем. Можете слати податке овом API-ју и добијати предвиђања која враћа модел.

Модел се деплојује коришћењем методе [deploy](https://docs.microsoft.com/python/api/azureml-core/azureml.core.model(class)?view=azure-ml-py#deploy-workspace--name--models--inference-config-none--deployment-config-none--deployment-target-none--overwrite-false--show-output-false-?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109).

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

Овај корак би треб
```python
response = aci_service.run(input_data=test_sample)
response
```  
Ово би требало да врати `'{"result": [false]}'`. То значи да је унос пацијента који смо послали на крајњу тачку генерисао предвиђање `false`, што значи да ова особа вероватно неће имати срчани удар.

Честитамо! Управо сте искористили модел који је постављен и обучен на Azure ML уз Azure ML SDK!

> **_NOTE:_** Када завршите пројекат, не заборавите да обришете све ресурсе.

## 🚀 Изазов  

Постоји много других ствари које можете урадити уз помоћ SDK-а, али нажалост, не можемо их све обухватити у овој лекцији. Добра вест је да учење како да прелиставате документацију SDK-а може вас далеко одвести. Погледајте документацију Azure ML SDK-а и пронађите класу `Pipeline` која вам омогућава да креирате цевоводе. Цевовод је збир корака који се могу извршити као радни ток.

**САВЕТ:** Идите на [документацију SDK-а](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) и унесите кључне речи у траку за претрагу, као што је "Pipeline". Требало би да добијете класу `azureml.pipeline.core.Pipeline` у резултатима претраге.

## [Квиз након предавања](https://ff-quizzes.netlify.app/en/ds/)

## Преглед и самостално учење  

У овој лекцији сте научили како да обучите, поставите и искористите модел за предвиђање ризика од срчане инсуфицијенције уз Azure ML SDK у облаку. Погледајте ову [документацију](https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py?WT.mc_id=academic-77958-bethanycheum&ocid=AID3041109) за додатне информације о Azure ML SDK-у. Покушајте да креирате сопствени модел уз Azure ML SDK.

## Задатак  

[Пројекат из науке о подацима уз Azure ML SDK](assignment.md)  

---

**Одрицање од одговорности**:  
Овај документ је преведен коришћењем услуге за превођење помоћу вештачке интелигенције [Co-op Translator](https://github.com/Azure/co-op-translator). Иако се трудимо да обезбедимо тачност, молимо вас да имате у виду да аутоматски преводи могу садржати грешке или нетачности. Оригинални документ на његовом изворном језику треба сматрати ауторитативним извором. За критичне информације препоручује се професионални превод од стране људи. Не преузимамо одговорност за било каква погрешна тумачења или неспоразуме који могу настати услед коришћења овог превода.