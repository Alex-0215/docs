---
title: "Контур.Диадок"
permalink: /docs/integration/diadoc/
toc: true
---

Сервис **Диадок** предназначен для обмена электронными документами через интернет.
Диадок позволяет компаниям мгновенно обмениваться любыми внешними и внутренними документами со своими клиентами,
поставщиками, партнерами, удаленными подразделениями.

Все электронные документы в сервисе подписаны электронной подписью и обладают юридической силой.

Дополнительная информация о Диадок здесь:
  - [Руководство пользователя сервиса Диадок](https://wiki.diadoc.ru/pages/viewpage.action?pageId=720902)
  - [Форматы электронных документов](https://www.diadoc.ru/docs)


**АРК: Транспортная логистика Online** позволяет выгружать в Диадок следующие документы:

| Документ              | Формат | Получение статуса из Диадок |
| --------------------- | ------ | --------------------------- |
| Счета на оплату       | PDF    | Да                          |
| Акт + счет-фактура    | XML    | Да                          |
| УПД                   | XML    | Да                          |
| Отчет экспедитора     | PDF    | Да                          |
| Акт сверки с клиентом | PDF    | Да                          |
|--------------------------------------------------------------|

## Получение доступа в Контур.Диадок
Если Ваша компания еще не имеет доступа к Диадок, зайдите на сайт [diadoc.kontur.ru](https://diadoc.kontur.ru)
и зарегистрируйтесь.

![](/assets/images/diadoc_contour.png)

## Подготовка к обмену с Диадок

### Настройка параметров доступа к API Диадок
В параметрах *АРК: Транспортная логистика Online* задайте:
  - *apiurl* = https://diadoc-api.kontur.ru:443
  - *apiclientid* = {id_diadoc}

![](/assets/images/diadoc_arc.png)

, где {id_diadoc} - идентификатор Диадок, полученный после заключения договора на использование API Диадок.

### Настройка нашей компании
В карточке *Нашей компании* на закладке *Настройки* в группе *Настройки Диадок* задайте:
  - *Логин Диадок* = {ВашПочтовыйЯщикДиадок}
  - *Пароль Диадок* = {ВашПарольОтПочтовогоЯщикаДиадок}

![](/assets/images/diadoc_password.png)   

## Работа с контрагентами в Диадок
*АРК: Транспортная логистика Online* позволяет обмениваться с клиентом документами,
если с ним установлена "дружба" в Диадок, т.е. он **является контрагентом** Вашей компании.

О том как подружиться с контрагетами, пишут здесь
[Работа с контрагентами](https://wiki.diadoc.ru/pages/viewpage.action?pageId=1146921).

## Настройка контрагента
**Важно!** Для использования ЭДО в карточке контрагента должен быть выбран ящик
Диадок с состоянием **Контрагент работает в Диадоке (Является контрагентом)**.

![](/assets/images/diadoc_counterparty.png)   

### Выбор ящика Диадок для контрагента
1) В меню *CRM* выберите пункт *Клиенты* и откройте карточку нужного контрагента.

![](/assets/images/diadok1.png)

Перейдите на вкладку *Внешние системы*.

![](/assets/images/diadok2.png)

Откройте вкладку *Диадок*.

![](/assets/images/diadok3.png)

При начальной настройке все поля пустые.

2) Для получения списка возможных ящиков используйте кнопку *Получить список...* на панели инструментов.

Автоматически заполнится список ваших компаний, с которыми у контрагента есть клиентский договор.

![](/assets/images/diadok4.png)

3) Для определения ящика Диадок для выбранной строки используйте кнопку *Указать ящик...* на панели инструментов.

В открывшейся форме поставьте флаг для того варианта, где состояние *Контрагент работает в Диадоке (Является контрагентом)*.
Кнопкой *Выбрать* сохраните выбранный вариант. Ящик контрагента для выбранной строки должен заполниться.

### Обновление состояния ящика Диадок для контрагента
Состояние отношений вашей компании и контрагента в Диадок могут измениться.

Для обновления состояния ящика Диадок для выбранной строки используйте кнопку *Обновить состояние...* на панели инструментов.

![](/assets/images/diadok5.png)
