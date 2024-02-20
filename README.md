# NP Сетевые системы и приложения - ВТОРОЙ СЕМЕСТР

# Страничка семинаров ПИ22-1 ПИ22-2 ПИ22-3 ПИ22-4




Основные темы практики:
---

Первый семестр:

* ~~[ОСНОВЫ LINUX](https://github.com/VladimirAndropov/fa-os-practice/README.md)~~



Второй семестр:

 * [Сетевые приложения](#брс) 




Материалы курса
---
Вы можете познакомиться со всеми материалами курса - презентациями к лекциям, методических рекомендациям к лабораторным работам на [github](http://koroteev.site/os/).

 Плейлист с видео по данному курсу досупен на [YouTube](https://www.youtube.com/playlist?list=PLhgyvraU60gU8OAhjtcipU_sO7UYvkQl9). 


# План семинарных занятий


- Системы контроля версий
  - Вначале мы изучаем git для совместной разработки
  - Учимся настраивать синхронизацию проектов через GitHub
 
- Использование сокетов
  - Затем создаем простейшее серверное приложение, которое отправляет потоковое видео

- Веб-сервер
  - Развиваем предыдущий опыт в сокетах до создания простейшего http веб-сервера 
  - Добавляем функционал многопоточности для http веб-сервера 
  - Добавляем функционал многопроцессности для ускорения http веб-сервера 
  - Добавляем библиотеки асинхронного программирования для http веб-сервера

- Развертывание сетевых приложений
  - В итоге пакуем в контейнер - развертываем http веб-сервер на удаленном ресурсе (hub.docker.com)



# БРС

<table border="0" cellspacing="0" cellpadding="0" class="Table1"><colgroup><col width="40"/><col width="479"/><col width="170"/></colgroup><tr class="Table11"><td style="text-align:left;width:0.924cm; " class="Table1_A1"><p class="P10"><span class="T2">№ </span></p><p class="P1"><span class="T2">п/п </span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A1"><p class="P11"><span class="T2">Вид учебной деятельности </span></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A1"><p class="P12"><span class="T2">Максимум  за семестр</span></p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A1"><p class="P4"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A1"><p class="P1">Второй семестр изучения дисциплины </span></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A1"><p class="P2"> </p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard"><span class="T3">Первая половина семестра</span></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13"> </p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">1. </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Аудиторная работа “Настройка рабочего окружения”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">2.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа DO2.1 “<a href="https://github.com/VladimirAndropov/0-git-basic" class="Internet_20_link"><span class="T4">Работа с Git в текстовом и графическом режиме</span></a>”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">3</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">3.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа DO2.2 “<a href="https://github.com/VladimirAndropov/fa-np-practice" class="Internet_20_link"><span class="T4">Работа с Git субмодули и синтаксис README.md</span></a>”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">2</p></td><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">4.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа “<a href="https://github.com/VladimirAndropov/1_echo_server" class="Internet_20_link"><span class="T4">TCP-потоковый сервер видео</span></a></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">3</p></td></tr>
<tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">5.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа “<a href="https://github.com/VladimirAndropov/2_threaded_server" class="Internet_20_link"><span class="T4">Многопоточный сервер на Python</span></a>” (основное задание)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">3</p></td></tr>
<tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">6.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа “<a href="https://github.com/fa-python-network/2_threaded_server" class="Internet_20_link"><span class="T4">Многопоточный сервер</span></a>” (основное задание и доп. п. 1)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">7.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа “<a href="https://github.com/VladimirAndropov/6_Web_server" class="Internet_20_link"><span class="T4">Веб-сервер HTTP</span></a>” (основное задание)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">3</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A3"><p class="Standard">8.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A3"><p class="Standard">Лабораторная работа “<a href="https://github.com/fa-python-network/3_Parallelism" class="Internet_20_link"><span class="T4">Использование параллельного программирования</span></a>” (основное задание и доп. пп. 1-2)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A3"><p class="P13">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard"><span class="T3">Вторая половина семестра</span></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P13"> </p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard">9.</p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Лабораторная работа “<a href="https://github.com/fa-python-network/6_Web_server" class="Internet_20_link"><span class="T4">Docker-контейнер</span></a>” (основное задание и доп. п. 1)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P13">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">10.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Лабораторная работа NT4.1 “<a href="https://docs.google.com/document/d/1yWW0frd1MdW0onBCcwQYSQk_NZWtkNSQ_f9uzCEbA0Q/edit?usp=sharing" class="Internet_20_link"><span class="T4">Docker-контейнер </span></a>”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">11.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Лабораторная работа NT4.2 “<a href="https://docs.google.com/document/d/1f89AvXRVuzqaAzMMqOzC1720OzYW3aziylDv6PX0SRE/edit?usp=sharing" class="Internet_20_link"><span class="T4">Балансировка нагрузки</span></a>”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">2</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">12.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Лабораторная работа “<a href="https://github.com/fa-python-network/5_FTP_server" class="Internet_20_link"><span class="T4">Docker-Composer”</span></a>” (основное задание)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">2</p></td></tr><tr class="Table141"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">13.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Лабораторная работа “Контейнеризация приложений курса”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">5</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">14.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="Standard">Аудиторная работа “VPN”</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">1</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">15.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="P1">Тестовые опросы на лекциях</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">5</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A11"><p class="Standard"><span class="T2">16.</span></p></td><td style="text-align:left;width:10.956cm; " class="Table1_A11"><p class="P1">Составление тестовых заданий (дополнительно)</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A11"><p class="P14">5</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A1"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A1"><p class="P3">Всего за семестр</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A1"><p class="P13">40</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A22"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A22"><p class="Standard"><span class="T3">Экзамен</span></p></td><td style="text-align:left;width:3.889cm; " class="Table1_A22"><p class="P13"> </p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A22"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A22"><p class="Standard">Решение практической задачи</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A22"><p class="P13">20</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A22"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A22"><p class="Standard">Теоретический опрос</p></td><td style="text-align:left;width:3.889cm; " class="Table1_A22"><p class="P13">40</p></td></tr><tr class="Table12"><td style="text-align:left;width:0.924cm; " class="Table1_A22"><p class="Standard"> </p></td><td style="text-align:left;width:10.956cm; " class="Table1_A22"><p class="P3">Всего за экзамен </p></td><td style="text-align:left;width:3.889cm; " class="Table1_A22"><p class="P13">60</p></td></tr></table>




# Примерные задания для подготовки к экзамену
1. Напишите программу, которая создает нить. Родительская и вновь созданная нити должны распечатать десять строк текста. [README](exam/1.md)
2. Напишите простой эхо-сервер, использующий неблокирующие сокеты и клиент к нему.[README](18sem-fs/socket_example.c)
3. Напишите простой многопоточный загрузчик URL. Список URL скрипт принимает как аргументы командной строки.[README](2017/20-socket/README.md)
4. Реализуйте простой HTTP-клиент. Он принимает один параметр командной строки - URL. Клиент делает запрос по указанному URL и выдает тело ответа на терминал как текст.
5. Напишите программу, которая вычисляет число Пи при помощи ряда Эйлера. Количество потоков программы должно определяться параметром командной строки. 
6. Дана функция calculate(x, y). Напишите программу, которая создает пул из 5 процессов и распределяет в этом пуле вычисление функции на промежутке х от 0 до 1 с шагом 0,1. у равняется 2 всегда.[README](2017/24-stdthread/README.md)
7. Напишите программу, которая проверяет все числа от 0 на простоту и выводит простые числа на экран по мере нахождения. Числа должны проверяться в различных потоках (или процессах, по выбору студента) Программа должна работать до тех пор, пока ее не остановит пользователь.
8. Напишите программу, которая обходит все файлы в директории, переданной ей как параметр и выводит на экран имена тех, чей размер задан как второй параметр. Реализовать рекурсивный обход поддиректорий.[README](12sem-fs/README.md)
9. Напишите программу, которая выводит на экран список номеров открытых портов на данной машине. Использовать команду netstat.
10. Напишите программу, которая копирует файл с удаленного хоста в текущую папку по SSH. Имя файла и адрес хоста принимать как параметры.


# Пример экзаменационного билета
Экзаменационный билет №

1. Понятие потокобезопасности. Причины, проблематика, способы обеспечения. (20 баллов)
2. Доступ к общим ресурсам в многопоточной программе. Механизмы блокировки ресурсов модуля threading. (20 баллов)
3. Напишите программу, которая создает четыре нити, исполняющие одну и ту же функцию. Эта функция должна распечатать последовательность текстовых строк, переданных как параметр. Каждая из созданных нитей должна распечатать различные последовательности строк. (20 баллов)

