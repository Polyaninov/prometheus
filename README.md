Домашнее задание к занятию 9.4 «Система мониторинга Prometheus»

В практике есть 3 основных и 2 дополнительных (со звездочкой) заданий. Основные задания нужно выполнять обязательно, со звездочкой - по желанию и его решение никак не повлияет на получение вами зачета по этому домашнему заданию, при этом вы сможете глубже и/или шире разобраться в материале.


Пожалуйста, присылайте на проверку все задачи сразу. Любые вопросы по решению задавайте в чате учебной группы.

Цели задания

Научитья создавать свои шаблоны в Zabbix, добавлять в Zabbix хосты и связывать шаблон с хостами

Научиться составлять кастомный дашборд

Научиться создавать UserParameter на Bash

Научиться создавать Python-скрип, добавляться в него UserParameter и прикреплять к шаблону

Научиться создавать Vagrant-скрипты для Zabbix Agent

Чеклист готовности к домашнему заданию

 Просмотрите в личном кабинете занятие "Система мониторинга Prometheus"
 
Инструкция по выполнению домашнего задания

Сделайте fork репозитория c шаблоном решения к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw).

Выполните клонирование этого репозитория к себе на ПК с помощью команды git clone.

Выполните домашнее задание и заполните у себя локально этот файл README.md:

впишите вверху название занятия и ваши фамилию и имя;
в каждом задании добавьте решение в требуемом виде: текст/код/скриншоты/ссылка;
для корректного добавления скриншотов воспользуйтесь инструкцией «Как вставить скриншот в шаблон с решением»;
при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в инструкции по MarkDown.

После завершения работы над домашним заданием сделайте коммит (git commit -m "comment") и отправьте его на Github (git push origin).

Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
Любые вопросы задавайте в чате учебной группы и/или в разделе «Вопросы по заданию» в личном кабинете.


Задание 1

Установите Prometheus.


Процесс выполнения

Выполняя задание, сверяйтесь с процессом, отражённым в записи лекции

Создайте пользователя prometheus

Скачайте prometheus и в соответствии с лекцией разместите файлы в целевые директории

Создайте сервис как показано на уроке

Проверьте что prometheus запускается, останавливается, перезапускается и отображает статус с помощью systemctl

Требования к результату

 Прикрепите к файлу README.md скриншот systemctl status prometheus, где будет написано: prometheus.service — Prometheus Service Netology Lesson 9.4 — [Ваши ФИО]

Ответ:


![Screenshot_31](https://user-images.githubusercontent.com/75700701/228632109-2514f82f-0a1f-495e-9a59-c1c3b89e21dd.png)


Задание 2

Установите Node Exporter.


Процесс выполнения

Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.

Скачайте node exporter приведённый в презентации и в соответствии с лекцией разместите файлы в целевые директории

Создайте сервис для как показано на уроке

Проверьте что node exporter запускается, останавливается, перезапускается и отображает статус с помощью systemctl
Требования к результату

 Прикрепите к файлу README.md скриншот systemctl status node-exporter, где будет написано: node-exporter.service — Node Exporter Netology Lesson 9.4 — [Ваши ФИО]
 
 Ответ: 
 
 Не могу понять, выдает ошибку но метрика открывается http://158.160.52.111:9100/
 
 ![Screenshot_33](https://user-images.githubusercontent.com/75700701/228654526-02ba5a02-a65d-4619-a319-8874d2463bcc.png)


![Screenshot_36](https://user-images.githubusercontent.com/75700701/228654970-56be5c04-fc80-44ba-bb5c-281d95d74ca3.png)



Задание 3

Подключите Node Exporter к серверу Prometheus.


Процесс выполнения

Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.

Отредактируйте prometheus.yaml, добавив в массив таргетов установленный в задании 2 node exporter

Перезапустите prometheus

Проверьте что он запустился

Требования к результату

 Прикрепите к файлу README.md скриншот конфигурации из интерфейса Prometheus вкладки Status > Configuration
 
 Прикрепите к файлу README.md скриншот из интерфейса Prometheus вкладки Status > Targets, чтобы было видно минимум два эндпоинта
 
 
 Ответ:
 

![Screenshot_35](https://user-images.githubusercontent.com/75700701/228652397-373ecac5-5bbc-4ec1-a250-59b61035da9f.png)


![Screenshot_34](https://user-images.githubusercontent.com/75700701/228652427-dc726cb5-a2bc-412c-afee-5b5b714f0adc.png)


