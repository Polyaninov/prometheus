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
 
 


