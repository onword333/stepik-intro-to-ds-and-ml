# Введение в Data Science и машинное обучение
Заметки [обучающего курса](https://stepik.org/course/4852/syllabus) платформы Stepik
[Основы статистики](https://stepik.org/course/76/promo)

## Словарь изученных методов Pandas
* filter() - отбор по колонок иил строк
* iloc() - выбирает строки и колонки
* loc() - выбор по лейблам
* groupby() - группировка данных
* aggregate() - агригация показателей
* rename() - переименование колонок
* assign() - добавляет новую колонку/и, только им и пользоваться т.к. он работает быстрее всех [подробнее](https://suilin.ru/post/pandas_column/)


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