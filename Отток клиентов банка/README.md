
# Описание проекта


Из банка стали уходить клиенты каждый месяц. Спрогнозирована вероятность ухода клиента из банка в ближайшее время.

Построена модель с предельно большим значением F1-меры с последующей проверкой на тестовой выборке. Доведена метрика до 0.59. 

Дополнительно измерен AUC-ROC, соотнесен с F1-мерой.

Обучение с учителем. Работа с несбалансированными данными.

### Задачи проекта
Анализ оттока клиентов из банка для выбор стратегии (удержание старых клиентов или привлечение новых клиентов).

### Ключевые слова и навыки
data science, machine learning, ML, Python, SQL, Git, Pandas, Numpy, Matplotlib, seaborn, Sklearn, Tableau, Spark, Hadoop, R, sci-py, Research, Kaggle, Algorithms, PyTorch, TensorFlow, CatBoost, xgboost, Support vector machines, градиентный бустинг, нелинейная оптимизация, кластеризация, random forest, descision trees,  regression,  Reinforcement Learning, OpenCV, PIL

### Описание данных

Данные находятся в файле `/datasets/Churn.csv`
Источник данных: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

Признаки:
* `RowNumber` — индекс строки в данных
* `CustomerId` — уникальный идентификатор клиента
* `Surname` — фамилия
* `CreditScore` — кредитный рейтинг
* `Geography` — страна проживания
* `Gender` — пол
* `Age` — возраст
* `Tenure` — количество недвижимости у клиента
* `Balance` — баланс на счёте
* `NumOfProducts` — количество продуктов банка, используемых клиентом
* `HasCrCard` — наличие кредитной карты
* `IsActiveMember` — активность клиента
* `EstimatedSalary` — предполагаемая зарплата

Целевой признак
* `Exited` — факт ухода клиента


# Содержание <a name="title"></a>

[Импорт библиотек и задание констант](#import)
1. [Загрузка и анализ данных](#1)

 
2. [Подготовка данных](#2)


    
3. [Обучение моделей](#3)

    3.1 [Обучение модели линейной регрессии](#3.1)
    
    3.2 [Обучение модели CatBoostRegressor](#3.2)

    3.3 [Обучение модели LightGBM](#3.3)


4. [Тестирование](#4)
