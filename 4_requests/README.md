# Postman & библиотека requests

Цель: написать клиента к ruz.fa.ru

Ход работы:
1) скачать \установить \запустить Postman
2) импортировать \ открыть в Postman файл 4_requests/ruz.fa.ru.postman_collection.json 
3) выполнить Get-запросы
4) найти вкладку code в Postman \ сгенерировать Python код c request
______

# Get-запросы

## Запрос id преподавателя

https://ruz.fa.ru/api/search?term=Андропов&type=person



![](img/2024-02-19_07-06-42.png)
_____
## Запрос id группы


https://ruz.fa.ru/api/search?term=ПИ22-3&type=group
![](img/2024-02-19_07-08-00.png)
______
## Запрос предметов по id группы

https://ruz.fa.ru/api/schedule/group/110929?start=2024.02.21&finish=2024.02.21

![](img/2024-02-19_07-09-20.png)
__________
## Запрос id аудитории

https://ruz.fa.ru/api/search?term=ауд.3310&type=auditorium


![](img/2024-02-19_07-29-24.png)
________

https://ruz.fa.ru/api/schedule/auditorium/2921?start=2024.02.21&finish=2024.02.21&lng=1

![](img/2024-02-19_07-31-44.png)
________
## Запрос id здания по адресу

https://ruz.fa.ru/api/search?term=Вешняковский проезд&type=building

![](img/2024-02-19_07-34-27.png)
_________
https://ruz.fa.ru/api/schedule/building/51?start=2024.02.21&finish=2024.02.21&lng=1

![](img/2024-02-19_07-38-19.png)