# project_wine

## План 
- [**Шаг 1.** Выбор темы](https://github.com/sashagrr/project_wine#%D0%B2%D1%8B%D0%B1%D0%BE%D1%80-%D1%82%D0%B5%D0%BC%D1%8B-%D0%B8-%D1%81%D0%B1%D0%BE%D1%80-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
- [**Шаг 2.** Сбор данных](https://github.com/sashagrr/project_wine#%D0%B2%D1%8B%D0%B1%D0%BE%D1%80-%D1%82%D0%B5%D0%BC%D1%8B-%D0%B8-%D1%81%D0%B1%D0%BE%D1%80-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
- [**Шаг 3.** Предварительная обработка данных](https://github.com/sashagrr/project_wine#%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F-%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
- [**Шаг 4.** Визуализция](https://github.com/sashagrr/project_wine#%D0%B2%D0%B8%D0%B7%D1%83%D0%B0%D0%BB%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F)
- [**Шаг 5.** Создание новых переменных и обработка уже существующих](https://github.com/sashagrr/project_wine#%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BD%D0%BE%D0%B2%D1%8B%D1%85-%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D1%85-%D0%B8-%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0-%D1%83%D0%B6%D0%B5-%D1%81%D1%83%D1%89%D0%B5%D1%81%D1%82%D0%B2%D1%83%D1%8E%D1%89%D0%B8%D1%85)
- [**Шаг 6.** Тестирование гипотиз](https://github.com/sashagrr/project_wine#%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B3%D0%B8%D0%BF%D0%BE%D1%82%D0%B5%D0%B7)
- [**Шаг 7.** Машинное обучение](https://github.com/sashagrr/project_wine#%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D0%BD%D0%BE%D0%B5-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5)

### Команда
- Гравер Александра 
- Масловская Анастасия
 
### Выбор темы и сбор данных
Вино с нами уже около 7000 лет, оно имеет большое социальное и экономиечское значение в современном мире. Династии делают производство этого напитка делом своей жинзи, страны богатеют, развивая данную отрасль. Вино - третий по полурности алкогольный напиток в мире и имеет один из самых сложных химических составов. Именно поэтому темой нашего проекта стал данный вид алкоголя. 
Мы выбрали датасет "Wine quality" с рекомендованного нам сайта Kaggle, с помощью которого мы хотели бы выяснить, как те или иные химические элементы влияют на качество вина. 
Задача проекта: проанализировать датасет, который содержит в себе набор данных о химических характеристиках разнличных вин, а также выявить закономерности с помощью визуализации исходных данных и тестировании различных гипотез. 
> данные можно найти в нашем репозитории

#### Ожидаемые результаты
Мы хотим, проанализировав имеющиеся данные с помощью методов машинного обучения, построить модель, которая предсказывала бы оценку качества вина на основе его химических характеристик. 

### Предварительная обработка данных

##### Описание переменных

###### Категориальная переменная: 

- __type__ - тип вина (белое или красное)

###### Количественные переменные: 

- __fixed acidity__ - фиксированная кислотность; данный тип кислот участвует в сбалансированности вкуса вина, привносит свежесть вкусу; с точки зрения процентного содержания кислоты, вино будет иметь кислотность от 0,6 до 0,7%. В данном датасете единица измерения г/дм3.

- __volatile acidity__ - летучая кислотность; является мерой газообразных кислот вина; количество летучих кислот в вине часто считается показателем порчи. В среднем белых вин 1,2 г/л и 1,75 г/л для красных. В данном датасете единица измерения г/дм3.

- __citric acid__	- лимонная кислота; является продуктом брожения виноградного сусла или мезги; до 2 г/дм3

- __residual sugar__ - остаточный сахар; характеристика, показывающая количество сахара, который не был превращен в спирт в процессе ферментации вина; до 40 г/дм3. В данном датасете измеряется в процентах.

- __chlorides__ - хлориды; характеризует бактериостатические и бактерицидные свойства вина. В данном датасете единица измерения г/дм3.

- __free sulfur dioxide__	- свободный диоксид серы (диоксид серы, готовый вступить в реакцию, то есть стабилизировать вино); пищевая добавка, выполняющая функции консерванта

- __total sulfur dioxide__ -  суммарный диоксид серы

- __density__	- плотность; определяется в первую очередь концентрацией спирта и сахара. Белые, розовые и красные вина, как правило, легче воды — их плотность при температуре 20°С ниже 998,3 кг/м 3

- __pH__ - кислотность; отвечает за способность напитка долго храниться и за его сочетаемость с различными блюдами; обычно колеблется в пределах 2,8-3,5

- __sulphates__ - сульфаты; сульфаты меди и железа применяются виноградарями на стадии выращивания винограда для обработки лозы от болезней. Эти химические элементы в напитке предназначены для сохранения в продукте вкуса, цвета и запаха.

- __alcohol__	- спирт; содержание в вине варьируется в пределах 4,5%-15%, а в крепленых — до 20%. 

###### Целевая переменная:

- __quality__ - оценка качества от 0 до 10

### Визуализация
> Результаты визуализации наших данных можно увидеть в тетрадке 

### Создание новых переменных и обработка уже существующих
В датасете очень много данных, значения которых выражены дробными, малоотличающимися величинами, поэтому мы решили провести категоризацию некоторых признаков в зависимости от интервала, в который поподает значение. Для этого мы создали из уже существующих признаков один новый - acidity и провели данную процедуру. Также разбили на категории вино по переменной residual sugar, и результаты записали в столбец sugar type. Признак quality решиили сделать бинарным, 0 - некачественное вино, 1 - качественное. 
Изучив, то на какие именно свойства вина влияют различные химические элементы, мы пришли к выводу о том, что наиболее существенным для нашего исследования будет соотношение кислотности и сахара, так как имнно оно в значительной стпенени имеет влияние на вкус, аромат, степень алкогольности и способность вина храниться.

### Тестирование гипотез

Мы сформулировали некоторые гипотезы, которые хотели бы проверить.  Для более полного понимая того, что именно мы будем тестировать в своей работе, мы записали основную гипотезу и альтернативную. Звучат они следующим образом: 

1. Вино с терпким вкусом и вино с мягким вкусом одинаково часто встречается среди качественных вин
 H0: вино с терпким вкусом и вино с мягким вкусом одинаково чсто встречается среди качественных вин\
 H1: терпкие вина чаще считаются качественными\
2. В среднем у качественных вин плотность ниже, чем у некачественных\
 H0: математическое ожидание плотности некачественных вин = математическому ожиданию плотности качественных вин\
 H1: математическое ожидание плотности некачественных вин больше математического ожидания плотности качественных вин\
3. Вино с более высоким содержанием спирта будет иметь более высокую оценку качества\
 H0: математическое ожидание оценки вина с более высоким содержанием спирта = математическому ожиданию оценки вина с низким содержанием спирта\
 H1: математическое ожидание оценки вина с более высоким содержанием спирта больше математичского ожидания оценки вина с низким содержанием спирта

### Машинное обучение
В нашей работе мы обучали алгоритмы логистической регрессии и случайного леса. 
Так же мы рассчиатли точность классификатора логистической регрессии на тестовом наборе и ROC-AUC. У нас поличились следеющие значения:
 - accurancy: 0.81
 - ROC-AUC: 0.62

## Заключение

### Полученные результаты

### Вывод
