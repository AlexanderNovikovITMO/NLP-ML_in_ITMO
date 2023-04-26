# NLP-ML_in_ITMO
Анализ естественного языка методами машинного обучения

Я выбрал набор данных для исследования: скачал с сайта kaggle набор данных Fake/Real Job Posting in Nigeria (https://www.kaggle.com/datasets/oyelajairemide/fakereal-job-posting-in-nigeria). 
Как заявено на сайте: «This is a compiled dataset consisting of over 200 real and fake job postings in Nigeria. This dataset is a valuable resource for anyone interested in analyzing the job market in Nigeria. This file has information about job descriptions. The label classifier, fake and real can be found in the "label" column as 1 and 0 respectively.»
Визуальный анализ данных (благо их не очень много) позволил сделать вывод, что проблем (пропусков, не читаемых символов и т.п.) в них не было.
С помощью data['label'].value_counts() я проверил выборку на сбалансированность: из 202 примеров 135 являются реальными, а 67 - фейками, так что, я предполагаю, что выборка является достаточно сбалансированной.
Затем я решил задачу классификации: выбрал метрику и построил бейзлайн.
Константное предсказание сработало, судя по метрикам, не очень хорошо, а вот логистическая регрессия - просто замечательно :)
