# Тестовое задание для компании Saber Interactive (вакансия аналитик данных)



***СТАТУС:*** **Завершён**


## Цели проекта:

Необходимо выполнить тестовое задание, включающее в себя составление двух SQL запросов на основе имеющихся данных и создание интерактивного приложения с помощью одного из веб фреймворков (streamlit/dash/panel) по макету.

## Задачи:

### SQL 1:

Напишите запрос, который выведет, сколько времени в среднем задачи каждой группы находятся в статусе “Open” 
Условия:
Под группой подразумевается первый символ в ключе задачи. Например, для ключа “C-40460” группой будет “C”
Задача может переходить в один и тот же статус несколько раз.
Переведите время в часы с округлением до двух знаков после запятой.

#### Результат выполнения задания SQL 1:

<img src="https://i.imgur.com/VDryupk.png" alt="SQL1"/>

### SQL 2:

Напишите запрос, который выведет ключ задачи, последний статус и его время создания для задач, которые открыты на данный момент времени.
Условия:
Открытыми считаются задачи, у которых последний статус в момент времени не “Closed” и не “Resolved”
Задача может переходить в один и тот же статус несколько раз.
Оформите запрос таким образом, чтобы, изменив дату, его можно было использовать для поиска открытых задач в любой момент времени в прошлом
Переведите время в текстовое представление

#### Результат выполнения задания SQL 2:

<img src="https://i.imgur.com/A1Oj2vi.png" alt="SQL2"/>

Получилось 40 строк незакрытых задач.

### Задание Python:

Создайте интерактивное приложение с помощью одного из веб фреймворков (streamlit/dash/panel), по следующему макету.
Исторические данные и список активов необходимо получить с помощью апи:  https://docs.coincap.io/

Макет:

<img src="https://i.imgur.com/1xdHWwq.png" alt="Python_ex"/>

#### Результат выполнения задания Python:

В своем варианте решения я использовал фреймворк dash.

<img src="https://i.imgur.com/kylSVMg.png" alt="Python_Mine"/>

Мой вариант графика показывает точки максимума и минимума за выбранный диапазон дат, а также позволяет переключать сами даты и валюту. Модель имеет дополнительный интерактивный разрез для приближения и отдаления графика.

Код ко всем задачам доступен в рамках данного репозитория.

## Инструменты проекта

- Python
- Pandas
- Sklearn
- Matplotlib.pyplot
- Dash
- SQLite3
