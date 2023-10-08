# Прогнозирование оттока клиентов телеком компании

[Telecom.ipynb](https://github.com/SvetBesedina/Portfolio-1/blob/main/Telecom/Telecom.ipynb)

## Описание проекта

На основе данных о клиентах (персональной информации, подключенных услугах, тарифах и договорах) предсказать вероятность их ухода с целью оптимизации маркетинговой политики и увеличения прибыли компании. 

## Навыки и инструменты

- **python**
- **pandas**
- **numpy**
- **datetime**
- sidetable

- **matplotlib**
- **seaborn**
- **scikitplot**

- **phik**.report.**lot_correlation_matrix**
- sklearn.metrics.**mutual_info_score**
- imblearn.pipeline.**make_pipeline**
- sklearn.pipeline.Pipeline
- sklearn.compose.**ColumnTransformer**
- imblearn.over_sampling.**SMOTE**
- sklearn.model_selection. (**RandomizedSearchCV**, **train_test_split**)
- sklearn.utils.class_weight.**compute_class_weight**
- sklearn.preprocessing. (**OneHotEncoder**, **OrdinalEncoder**, **StandardScaler**)
  
- sklearn.linear_model.**LogisticRegression**
- sklearn.ensemble.**RandomForestClassifier**
- lightgbm.**LGBMClassifier**
- catboost.**CatBoostClassifier**
- sklearn.metrics. (accuracy_score, roc_auc_score, f1_score,
                    precision_score, recall_score, precision_recall_curve)                                                                    

## Вывод

Была проведена исследовательская работа по анализу исторических данных о клиентах компании, а также обучение и выбор модели прогнозирования оттока клиентов. Были построены пайплайны для моделей логистической регрессии, случайного леса, LightGBM и CatBoost с подбором гиперпараметров и кроссвалидацией в процессе обучения. Для целей предсказания вероятности ухода клиента была выбрана модель CatBoost как более устойчиво дающая наибольшую метрику ROC-AUC. 
Выведена таблица с показателем вероятности ухода по каждому человеку из списка клиентов тестового набора данных. На основании данной величины можно сгруппировать «отточных» клиентов и каждой группе предложить различные системы скидок, провести оптимизацию маркетинговой политики, предлагаемых клиенту продуктов и условий сотрудничества.

Имея выгрузку данных по клиентам, которые склонны к оттоку, можно уже рассчитать альтернативные издержки на предоставление скидки и упущенную выгоду от ухода клиента с проведением соответствующего анализа и составлением прогнозов для компании в обоих случаях. Таким образом, можно добиться сокращения неоптимальных расходов компании и целенаправленной точечной работой с отдельными группами клиентов.
