# Сервис для чтения книг

**Цель исследования:**
Проанализировать базу данных. В ней — информация о книгах, издательствах, авторах, а также пользовательские обзоры книг. Эти данные помогут сформулировать ценностное предложение для нового продукта.
С помощью SQL-запросов решить задания.

**Задания**

- Посчитайте, сколько книг вышло после 1 января 2000 года;
- Для каждой книги посчитайте количество обзоров и среднюю оценку;
- Определите издательство, которое выпустило наибольшее число книг толще 50 страниц — так вы исключите из анализа брошюры;
- Определите автора с самой высокой средней оценкой книг — учитывайте только книги с 50 и более оценками;
- Посчитайте среднее количество обзоров от пользователей, которые поставили больше 48 оценок.

**Этапы исследования:**

- Доступ к базе данных;
- Исследование данных;
- Решение задач;
- Выводы.

**Навыки и инструменты:**
- pandas
- sqlalchemy

**Общий вывод:**
В результе проделанной работы получили следующие выводы:
- После 1 января 2000 года вышло 819 книг. Учитывая тот так что всего книг 1000 можно сказать что это практически 82% от всего списка.
- Для подсчета использовали две отдельные таблицы, после чего с помощью джойна объединили оценки и обзоры со списком книг. И получили таблицу с количеством обзоров и средним рейтингом для всех книг. При этом если выбрать рейтинг равный 5, получим что у нас таких целых 43 книги.
- Наибольшее число книг толще 50 страниц опубликовало издательство Penguin Books. Было издано 42 книги.
- Cамую высокую оценку имеет J.K. Rowling/Mary GrandPré. Оценка 4,28, при этом количество оценок 310.
- А среднее количество обзоров пользователей кто поставил более 48 оценок равно 24. Что говорит нам о том что пользователи кто оставляет оценки так же охотно оставляют обзоры книг.

После получения информации по задачам можно сказать о том, что пользователи продолжают читать. При этом не только оценивать книги, но и оставлять на них свои обзоры, что очень важно и помогает в подборе интересной книги. Считаю что стоит подумать в направлении того чтобы максимально поощрять пользователей делится своим мнение о прочитанных книгах. Так как на освновании имеющихся оценок и обзоров можно собрать рекомендации для других пользователей.