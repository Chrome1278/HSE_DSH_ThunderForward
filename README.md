# HSE DSH ThunderForward

## Постановка задачи
Нашей задачей является оценка этической репутации банков на основе текстовой информации — отзывов клиентов банков, оставленных на различных онлайн-площадках.
Этическая репутация в целом схожа с общим сентиментом (хорошо-плохо), но фокусируется только на этичности банка, то есть на том, насколько банк ведет себя хорошо в этическом смысле (соблюдает этические нормы - не обманывать, не злоупотреблять властью, быть вежливым и т. д.). Например, если пользователю нравится дизайн карты или офиса банка, это не будет иметь никакого отношения к этическому сентименту. Но во многих случаях общий сентимент по отношению к банку является по сути этическим сентиментом, поскольку потребителю может нравиться, что с ним вежливо разговаривали, не обманули его, не задирали цены, не халтурили с качеством и т. п., что и является соблюдением этических
норм бизнеса.

## Подготовка данных
В процессе подготовки данных был изучен предосталвенный датасет. Были обнаружены дубликаты текстов с различающимися размеченными классами, эти дубликаты были объеденены опираясь на имеюущуся перекрестную разметку, после чего тексты были отфильтрованы по значению уверенности размеченного класса.

## Разведочный анализ данных
В процессе разведочного анализа данных мы рассмотрели данные с целью найти в них закономерности и увидеть распределения. Ноутбук с результатами и выводами представлен [по ссылке](https://github.com/Chrome1278/HSE_DSH_ThunderForward/blob/main/eda.ipynb).

## Методы решения
В ходе хакатона наша команда применила два подхода для решения поставленной задачи:
1. Методы глубокого обучения с использованием нейронной сети на основе архитектуры трансформер.
2. С использованием классических алгоритмов машинного обучения (**лучшее решение**).

### Нейронные сети
Мы использовали предобученную на финансовом корпусе данных [модель](https://huggingface.co/ProsusAI/finbert), которая предсказывает тональность предложения. Мы дообучили эту модель на предоставленных данных, однако нам не удалось получить высоких результатов. Лучшим результатом для этой модели было 0.7 по метрике F1 Score. 

### Машинное обучение

### Сравнение

## Заключение

## Стек технологий
