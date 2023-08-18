# Введение в Data Science и машинное обучение
Заметки [обучающего курса](https://stepik.org/course/4852/syllabus) платформы Stepik
[Основы статистики](https://stepik.org/course/76/promo)

[Открытые базы данных](https://jivoi.github.io/2015/07/04/otkrytyie-bazy-dannykh-rf/)

[kaggle](https://www.kaggle.com/)

[Сообщество Open Data Science](https://ods.ai/jobs)

[Посещать data fest, как попасть](https://youtu.be/w-0NdY8y-4Y?t=2482)

[X5 Tech, Валерий Бабушкин](https://www.youtube.com/@X5Technology/featured)

[Hadoop - разработка и выполнение распределённых программ, работающих на кластерах из сотен и тысяч узлов](https://hadoop.apache.org/)

## Контакты
* [Валерий Бабушкин](https://youtu.be/w-0NdY8y-4Y), [vk](https://vk.com/venheads)
* [Мария Жавадова](https://youtu.be/SMRI4qKgyq8), [vk](https://vk.com/zhavadik)
* [Анатолий Карпов](https://t.me/karpov_anatoly)

## Словарь изученных методов Pandas
* filter() - отбор по колонок иил строк
* iloc() - выбирает строки и колонки
* loc() - выбор по лейблам
* groupby() - группировка данных
* aggregate() - агригация показателей
* rename() - переименование колонок
* assign() - добавляет новую колонку/и, только им и пользоваться т.к. он работает быстрее всех [подробнее](https://suilin.ru/post/pandas_column/)
* fillna() - заполняет значения NA/NaN указанными значениями
* median() - возвращает медиану значений по указаной оси
* to_datetime() - конверирование в объект даты и времени datetime64. Работа с датой [пример1 ](https://python-scripts.com/datetime-time-python), [пример 2](https://www.geeksforgeeks.org/python-working-with-date-and-time-using-pandas/), [пример 3](https://medium.com/datadriveninvestor/how-to-work-with-dates-in-pandas-like-a-pro-a84055a4819d)

## Форматирование даты
    %d — день месяца (от 01 до 31)
    %m — номер месяца (от 01 до 12)
    %Y — четырёхзначный номер года (например, 2019)
    Z или T — стандартный разделитель даты и времени
    %H — номер часа в 24-часовом формате
    %I — номер часа в 12-часовом формате
    %M — минуты (от 00 до 59)
    %S — секунды (от 00 до 59)
    'D' — *day (*от англ. «день»)
    'H' — hour (от англ. «час»)
    'min' или 'T' — minute (от англ. «минута»)
    'S' — second (от англ. «секунда»)

## Визуализация
* [matplotlib](https://matplotlib.org/)
* [встроенная в pandas визуализация](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.plot.html)
* [seaborn](https://seaborn.pydata.org/)

### Графики
* DataFrame.hist() - гистограмма
* DataFrame.plot.scatter() - точечная диаграмма, корреляция между двумя переменными
* seaborn.kdeplot - график плотности
* seaborn.displot - эта функция обеспечивает доступ к нескольким подходам к визуализации одномерного или двумерного распределения данных. Параметр kind - определяет, что рисуем.
* seaborn.pairplot - отражающий зависимость пар переменных друг от друга, а также распределение каждой из переменных

## Карьера в data science
Тезисы из видео:

1. При построении карьеры в Data Science важно иметь готовые проекты, чтобы на собеседовании направить диалог по удобному для себя руслу, да и просто продемонстрировать свои конкурентные преимущества

2. Датасеты для анализа можно брать с kaggle, открытых источников, или просто собирать при помощи парсеров. причём последний вариант даёт плюс к компетенциям, поскольку вы покажете умение кодить и получать данные для своих моделей

3. Важны soft-skills

4. Важно и нужно уметь отвечать на вопросы не "Сколько?", а "Почему?". Поскольку получение цифр не даёт информации, а анализ этих цифр, анализ причин почему цифры именно такие, и как они сформировались - позволяет представить некоторую картину в процессах.

5. Работайте с API и хакатонами. Поднатаскайтесь в плане работы с проектами, пусть даже через API проекта. Пишите свои проекты и ссылайтесь на них в резюме.

## Карьера аналитик
Требования:
* python (база)
* sql (база)
* иметь опыт работы с данными
* в завис. на какую поз. претендует - решать аналитические задачи. 
    
    Для junior:
    1. доставать данные
    2. посчитать средн. чек.
    3. посчитать ретеншн (понять как посчитать вручную)
    4. сред. врем. посещения сервиса
    5. посчитать черн
    6. подготовка А/Б тесты (проверить какиде данные нужны, проверить что все пишется, после теста посмотреть на результат и объяснить его)
    7. Важное качествно аналитика - проверка гипотез быстро
    8. Сколько слов в русс. языке. Можно оценить по славарю, понять сколько слов на одной странице

Список вопросов от гугла на собеседование: сколкьо шариков поместится в автубус ?

### Что указывать в резюме
[Источник](https://youtu.be/SMRI4qKgyq8?t=3070)
1. Все курсы которые проходил
2. Если резюме пустовато, то добавить, что-то про решение задачи, про себя: что изучаешь, как развиваешься, в каких группах состоишь, какие задачи умеете решать (а/б тесты, вы нашли анамалию в каком-то датасете)
3. Пишете в личку, проявляйте вовлеченность


### Тестовая задача для junior аналитика
Есть график кол-ва комментариев из года в год. На графике видно, что с какого-то времени начался плавный рост кол-ва комментариев (в теч. года вырос на +50%). Также известно, что в отчетный период была внедрена новая система комментариев. Приходит pr служба к аналитику и говорит, что хотят сделать пресс релиз новой системы комментариев и что она повлияла на пользователей - они стали чаще их делать, проверьте, что все именно так, можем ли мы опубликовать ? 

Вопрос аналитику: почему это может быть нет так ? Вот график, он расчет, почему нет ?

Предположение:
Возможно мы возрасли из-за того, что боты начали комментить больше из-за того, что после внедрения была сломано ограничение по отправке сообщений на аккаунт (50 шт в день). Как проверить ?


Ответ: нужно проанализировать пользователей разбив их по кагортам. В одну кагорту взять тех кто отправлял больше 50 комментов в день, другая кагорта меньше 50. Если сломали лимиты, то у ботов этот график уйдет в небеса. В случае если все нормально, то у кагортов будет плавный рост.

[источник](https://youtu.be/SMRI4qKgyq8?t=1813)


## 1.2 Биг дэйта, дип машин лернинг, основные понятия
[Как попасть в data science](https://www.youtube.com/watch?v=lDkTNURDIaY)

Стадии машинного обучения:
1. Обозначить проблему которую необходимо решить
2. Предобработка данных (извлечение, чистка данных)
3. Применение машинного обучение (регресия, классификация)
4. Валидация модели (удостовериться что модель правильно предсказывает, как понять что есть проблема)

## 1.3 Модель, нет, не супермодель, начнем с дерева
Алгоритмы машинного обучения:
- линейная регрессия
- решающие деревья

Классификация и регрессия

![image](assets/image/Классификация%20и%20регрессия.png)

Задача регрессия - предсказание количественной переменной
Задача классификации - предсказание классов (например один из двух возмжных классв, запрещенный и не запрещенный багаж)

Модели машинного обучения:
- дерево решиений
- нейронные сети

## 1.4 Pandas, Dataframes, нет, панды тут ни при чем
Cheat Sheets по Python, Jupyter, NumPy, SciPy, Pandas, Scikit-Learn, Matplotlib, Seaborn и Bokeh.
[Одним pdf файлом](assets/python-cheatsheets.pdf)

[Статья про ML простым языком](https://vas3k.ru/blog/machine_learning/)
### Pandas
Основные способы выборки данных:
* iloc - выбирает строки и колонки
* loc - выбор по лейблам

[разница между pandas loc и iloc](https://stackoverflow.com/questions/31593201/pandas-iloc-vs-ix-vs-loc-explanation)

Как отобрать все строки кроме указанных [док-ция](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.drop.html) ответ на [stackoverflow](https://stackoverflow.com/questions/31593201/how-are-iloc-and-loc-different)

[](https://stackoverflow.com/questions/28256761/select-pandas-rows-by-excluding-index-number)
[Пример](assets/1_4_lesson.ipynb)

table_random['gender'] - вернет тип series

table_random[['gender']] - вернет тип dataframe

Сопоставьте значения из двух списков
![image](https://github.com/onword333/stepik-intro-to-ds-and-ml/assets/19665506/7a5c5572-28a2-46ce-aebd-e928009fd528)

## 1.5 Фильтрация данных
query - отбор данных

отбор по двум условиям

    data[(data['writing score'] > 74) & (data.gender == 'female')]
При работе с pandas series для логического И нужно использовать & вместо уже знакомого and. Нужно указать приоритет операций, взяв условия в скобки [(condition) и (condition)]

[notebook примеры урока](https://github.com/onword333/stepik-intro-to-ds-and-ml/blob/main/assets/1_5_lesson.ipynb)

[Как различается среднее и дисперсия оценок по предметам у групп студентов со стандартным или урезанным ланчем ?](assets/1_5_lesson.ipynb)

![image](assets/Шаг%207%20–%20Фильтрация%20данных%20–%20Stepik.jpg)

Сопоставьте значения
![image](assets/Шаг%209%20–%20Фильтрация%20данных.jpg)

### Отбор колонок, метод filter
filter - отбирает колонки по названию колонок или по строкам

    DataFrame.filter(items=None, like=None, regex=None, axis=None)

### Шаг 12
Отберите колонки, в которых есть '-' в датафрэйме df (вот соответствующий датасэт). Сохраните их в переменную selected_columns
    
    selected_columns = df.filter(like = '-')

## 1.6 Группировка и агрегация
groupby - группировка данных см. [пример](assets/1_6_lesson.ipynb)

Сгруппируйте героев из датасэта (dota_hero_stats.csv) по числу их ног (колонка legs), и заполните их число в задании ниже:

![image](assets/image/1_6_5.jpg)

К нам поступили данные из бухгалтерии о заработках Лупы и Пупы за разные задачи! Посмотрите у кого из них больше средний заработок в различных категориях (колонка Type) и заполните таблицу, указывая исполнителя с большим заработком в каждой из категорий: