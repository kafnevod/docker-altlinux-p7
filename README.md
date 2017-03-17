# docker-altlinux-p7
Docker image for altlinux p7 


---
title: Linux в ИВС
sidebar: devprocess_sidebar
keywords: hosting
toc: false
permalink: devprocess_altlinux.html
---

## Linux в ИВС

### Политика использования Linux-дистрибутивов в рамках ГК ИВС

Создаваемые в рамках ГИ ИВС Linux-решения в зависимости типа Заказчика можно разделить на следующие группы:

1. Сертифицированные по различным уровням ФСТЭК или ФСБ решения для коммерческих или государственных Заказчиков

2. Решения для государтственных Заказчиков 

3. Решения для коммерческих Заказчиков

### Сертифицированные по различным уровням ФСТЭК или ФСБ решения для коммерческих или государственных Заказчиков

Для этого класса решений допускаются к использованию только Linux-дистрибутивы имеющие сертификаты требуемых уровней.
На настоящий момент эти сертификаты имеют дистрибутивы (а алфавитном порядке):

Производитель | Дистрибутив | Дата сертификации | Дата окончания действия сертификата | Базовый дистрибутив | Версия ядра
--------------|-------------|-------------------|-------------------------------------|---------------------|------------
Базальт СПО   | Альт Линукс СПТ 6.0 | ФСТЭК 18.04.2011 | ФСТЭК 18.04.2017**  |  Собственная пакетная база | 2.6.32
Базальт СПО   | Альт Линукс СПТ 7.0 | ФСТЭК ** | ФСТЭК ** |  Собственная пакетная база | 3.14
АО «НПО РусБИТех» | Astra Linux Special Edition релиз "Смоленск" | Минобороны 24.09.2010, ФСТЭК 27.01.2012, ФСБ 09.09.2016  | Минобороны 15.09.2018, ФСТЭК 27.01.2018, ФСБ 31.08.2021  |  Debian | 4.2.0
НТЦ ИТ Роса| РОСА ХРОМ | ФСТЭК 28.01.2014 | ФСТЭК 28.01.2014 |  Собственная пакетная база | 3.0.69

** - В марте 2017 планируется получение сертификата на СПТ 7.0 и продление сертификата СПТ 6.0 

Таким образом из сертифицированных российских дистрибутивов в ближайшее время будут доступны дистрибутивы Astra Linux и ALTLinux.
Данные дистрибутивы сертифицированы на использование KVM-сиртуализации.
АО «НПО РусБИТех» планирует в этом году сертифицировать решение на базе KVM - [ПК «ВИУ» ]((http://www.astralinux.com/home/novosti/394-rbt-pkviu.html).
Данные дистрибутивы по техническим и сертификационным проблемам не поддерживают docker-конейнеризацию.
Ведутся переговоры с производятелямя дистрибутивов о возможности сертификации данного решения в разрабатываемых сертифицируемых дистрибутивов. 

В настоящее время на рынке есть сертифицированные ФСТЭК дистрибутивы RedHat, SLES. Цена их на порядок превышает российские (600 000 - 1 600 000 рублей).


### Решения для государтственных и муниципальных Заказчиков

Решения для государственных Заказчиков должны использовать ПО, включенное в [Реестр отечественного ПО](https://reestr.minsvyaz.ru/). 
В настоящее время допускается использование свободного программного обечпечения не включенные в реестр, но 
идея "Реестра отечественного ПО" заключается в в переводе компетенций по разработке ПО на российские компании.
Поэтому чем дальше, тем больше для гос предприятий будут зажимать лайзейку по использованию стороннего открытого ПО
так как это ПО в России никто не поддерживает. Появился даже термин «дикое СПО» для такого класса "немейнстрим" продуктов.

 В связи с этим целесообразно в решениях для государтственных и муниципальных Заказчиков использовать российские дистрибутивы, включенные в реестр отечественного ПО:

*  [Альт Рабочая станция](https://www.basealt.ru/products/alt-workstation/), [Альт Сервер](https://www.basealt.ru/products/alt-server/), [Альт Образование](https://www.basealt.ru/products/alt-education/);

* [АстраЛинукс](http://astralinux.ru/);

* [ОС РОСА](https://www.rosalinux.ru/support/download_manuals/)





### Решения для коммерческих Заказчиков

  
