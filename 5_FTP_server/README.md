

File Transfer using TCP Socket in Python
========================================


В этой статье мы реализуем известный протокол в компьютерных сетях, называемых File Transfer Protocol (FTP) using [Python](https://www.geeksforgeeks.org/python-programming-language/learn-python-tutorial/). Мы используем гнездо TCP для этого, то есть, ориентированное на соединение сокет. [FTP](https://www.geeksforgeeks.org/file-transfer-protocol-ftp-in-application-layer/) (File Transfer Protocol) Является сетевым протоколом для передачи файлов между компьютерами по протоколу управления передачей/Интернет -протокол ([TCP/IP](https://www.geeksforgeeks.org/tcp-ip-model/)) соединения.FTP **обычно используется для передачи файлов** за кулисами для других приложений, таких как **банковские услуги.**

> **Предварительные знания**:  [лаба 1](https://github.com/VladimirAndropov/1_echo_server)

**File Structure**

![File Transfer using TCP Socket in Python](https://media.geeksforgeeks.org/wp-content/uploads/20230328155128/Screenshot-from-2023-03-28-15-48-47.png)

### **TCP-SERVER.py: Реализация на стороне сервера**

Мы начинаем с импорта библиотеки сокетов и изготовления простого розетки. **AF\_INET** Относится к адресу адреса IPv4.А **SOCK\_STREAM** означает, ориентированный на соединение протокол TCP.После этого мы связываем адрес хоста и номер порта с сервером.  
Пользователь входит в **максимальное количество клиентских подключений, необходимых**. На основе ввода мы определяем размер хранения клиентов, которые придерживаются **подключения** .Это происходит до тех пор, пока массив соединений не достигнет своего максимального предела.Затем для каждого соединения начинается обработка,

*   Данные получены, а затем декодируются.
*   Если данные не являются нулевыми, сервер создает файл с именем «output.txt» и записывает его в него.
*   Это продолжается до тех пор, пока все данные не будут записаны в файл
*   Выше приведено для всех клиентов, а затем соединения закрыты.Следовательно, мы можем получить новый файл на конце сервера с одинаковыми данными.

Python3
-------
```python
import socket

if __name__ == '__main__':

    # Defining Socket

    host = '127.0.0.1'

    port = 8080

    totalclient = int(input('Enter number of clients: '))

    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

    sock.bind((host, port))

    sock.listen(totalclient)

    # Establishing Connections

    connections = []

    print('Initiating clients')

    for i in range(totalclient):

        conn = sock.accept()

        connections.append(conn)

        print('Connected with client', i+1)

    fileno = 0

    idx = 0

    for conn in connections:

        # Receiving File Data

        idx += 1

        data = conn[0].recv(1024).decode()

        if not data:

            continue

    # Creating a new file at server end and writing the data

        filename = 'output'+str(fileno)+'.txt'

        fileno = fileno+1

        fo = open(filename, "w")

        while data:

            if not data:

                break

            else:

                fo.write(data)

                data = conn[0].recv(1024).decode()

        print()

        print('Receiving file from client', idx)

        print()

        print('Received successfully! New filename is:', filename)

        fo.close()

    # Closing all Connections

    for conn in connections:

        conn[0].close()
```
________
### **TCP-CLIENT.py: Реализация на стороне клиента**

Сначала мы создаем сокет для клиента и подключаем его к серверу, используя кортеж, содержащий адрес хоста и номер порта.Затем пользователь вводит имя файла, которое он хочет отправить на сервер.После этого, используя функцию **open ()** Python, данные файла читаются.Данные считываются по строке по строке, а затем кодируются в двоичном файле и отправляются на сервер, используя **socket.send ().** При завершении отправки данных файл закрыт.Он продолжает запрашивать имя файла у пользователя, пока подключение клиента не будет прекращено.

Python3
-------
```python
import socket

# Creating Client Socket

if __name__ == '__main__':

    host = '127.0.0.1'

    port = 8080

    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

# Connecting with Server

    sock.connect((host, port))

    while True:

        filename = input('Input filename you want to send: ')

        try:

           # Reading file and sending data to server

            fi = open(filename, "r")

            data = fi.read()

            if not data:

                break

            while data:

                sock.send(str(data).encode())

                data = fi.read()

            # File is closed after data is sent

            fi.close()

        except IOError:

            print('You entered an invalid filename!\

                Please enter a valid name')
```

**Итог:**

Теперь мы запускаем сервер, используя команду.

        python tcp-server.py

![](https://media.geeksforgeeks.org/wp-content/uploads/20230327193359/serverside.png)

Вывод на стороне сервера

После этого мы указываем максимальное количество возможных клиентских соединений (скажем, 2).

*   **Clients’ connections are initialized,** то есть массив соединений генерируется размером 2 для хранения клиентов.
*   После этого мы создаем новый терминал и запускаем нашего клиента, используя команду.

        python tcp-client.py

Максимальное количество вкладок, где мы можем запустить команду в терминале.Таким образом, мы создаем двух клиентов клиента 1 и клиент 2.

![File Transfer using TCP Socket in Python](https://media.geeksforgeeks.org/wp-content/uploads/20230327193643/client-side.png)

Вывод на стороне клиента

Как только клиент запускается, мы видим вывод «**подключен с клиентом 1**» на стороне сервера, указывая, что соединение успешно завершено с первым клиентом.То же самое для второго клиента.
После этого, на стороне клиента, мы даем имя файла, которое хотим отправить.Здесь **file1.txt** отправляется обоими клиентами.Содержание **file1.txt** показано ниже:

![File Transfer using TCP Socket in Python](https://media.geeksforgeeks.org/wp-content/uploads/20230326204932/sent_file.png)

Файл отправлен на сервер

Обратите внимание, что на стороне клиента мы продолжаем показывать подсказку: “**Input filename you want to send:**” так что клиент может отправлять несколько файлов.Как только соединение с клиентом отключено, используя «Control+C» в терминале, новый файл с именем output.txt сгенерирован на стороне сервера с тем же контентом, и соединение закрыто.Здесь файл клиента 1 хранится как **Output0.txt,** и файл клиента 2 хранится как **Ouput1.txt.**

![File Transfer using TCP Socket in Python](https://media.geeksforgeeks.org/wp-content/uploads/20230326204736/file.png)

Файл, полученный от клиента 1

![](https://media.geeksforgeeks.org/wp-content/uploads/20230327194150/output1.png)

Файл, полученный от клиента 2

Если непонятно, есть [видюшка](https://media.geeksforgeeks.org/wp-content/uploads/20230328132228/New_Recording_-_27_03_2023_19_44_33.mp4)