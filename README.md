# OS-IHW3

# Алёшкина Милана Вадимовна, БПИ-216
## ИДЗ № 3, Вариант 12

***Задача о гостинице – 1***

В гостинице 30 номеров, гости гостиницы снимают номер на одни или несколько суток. Если в гостинице нет свободных номеров, гости не уходят, а устраиваются рядом с гостиницей на скамейках и ждут, пока любой номеров не освободится.

*Создать приложение, моделирующее работу гостиницы. Сервер — это гостиница. Прибывающие гости могут порождаться отдельным клиентом. Другой клиент — это скамейки, образующие очередь ожидающих гостей.*


***Отчет на 4 - 5 баллов***

Сценарий работы программы:

Запускается сервер hotel и клиенты: visitors и street.

В hotel в качестве аргументов командной строки можно передать номер порта; в visitors в качестве аргументов командной строки нужно передать адрес ip и порт сервера; в street в качестве аргументов командной строки нужно передать адрес ip и порт сервера, количество посетителей.

hotel контролирует время, на которые заняты номера, а также то, какие посетители в них проживают.

visitors отвечает за алгоритм поведения посетителей.

street контролирует список ожидающих посетителей.

После старта всех процессов visitors запрашивает у hotel информацию о ожидающих посетителях -- hotel получает эту информацию у street и отправляет visitors. Если ожидающих пользователей нет, то visitors сообщает hotel об окончании работы. В ином случае для каждого из ожидающих пользователей visitors делает запрос на свободную комнату в hotel, если такая есть, то делает запрос на занятие данной комнаты данным посетителем (visitors пробрасывает информацию о посетителе, занявшем комнату, в street). После обработки всех пользователей visitors сообщает об этом в hotel, который в свою очередь проводит ревизию номеров.

[Программа живет в этом домике](https://github.com/milashkinaa/OS-IHW3/tree/main/4-5%20points)

***Отчет на 6 - 7 баллов***

Сценарий работы программы:

Запускается сервер hotel и клиенты: visitors, street и display.

В hotel в качестве аргументов командной строки можно передать номер порта; в visitors и display в качестве аргументов командной строки нужно передать адрес ip и порт сервера; в street в качестве аргументов командной строки нужно передать адрес ip и порт сервера, количество посетителей.

hotel контролирует время, на которые заняты номера, а также то, какие посетители в них проживают.

visitors отвечает за алгоритм поведения посетителей.

street контролирует список ожидающих посетителей.

display ведёт логгирование всего процесса работы отеля.

После старта всех процессов visitors запрашивает у hotel информацию о ожидающих посетителях -- hotel получает эту информацию у street и отправляет visitors. Если ожидающих пользователей нет, то visitors сообщает hotel об окончании работы. В ином случае для каждого из ожидающих пользователей visitors делает запрос на свободную комнату в hotel, если такая есть, то делает запрос на занятие данной комнаты данным посетителем (visitors пробрасывает информацию о посетителе, занявшем комнату, в street). После обработки всех пользователей visitors сообщает об этом в hotel, который в свою очередь проводит ревизию номеров.

Обо всех производимых действиях hotel сообщает в display, который выводит полученнную информацию на экран.

[Программа живет в этом домике](https://github.com/milashkinaa/OS-IHW3/tree/main/6-7%20points)

***Компиляция:***

cmake . -B build &&

cmake --build build --target all

***Традиция***

Как вы помните, в моих отчетах всегда были собачки. Этот отчет - не исключение. Наслаждайтесь. Это вам.

![Смотрите, какая красивая!](https://i.pinimg.com/564x/c8/2d/fc/c82dfcd58a3bd41b3bd9635cab0acaa9.jpg)

