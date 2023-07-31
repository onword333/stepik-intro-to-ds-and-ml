# Введение в Data Science и машинное обучение
Заметки [обучающего курса](https://stepik.org/course/4852/syllabus) платформы Stepik

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

![image](https://github.com/onword333/stepik-intro-to-ds-and-ml/assets/19665506/f856868a-21c4-4fd1-82e6-04149cc6a5fd, "Классификация и регрессия")

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
