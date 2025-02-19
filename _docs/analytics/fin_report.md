---
title: "ФинОтчет"
permalink: /docs/analytics/fin_report/
toc: false
---

## Как работает финотчет
1. Финотчет формируется из доходов (суммы клиенту) и расходов (суммы поставщикам), **привязанных** к финпериоду (отчетный месяц)
2. В момент формирования счета-фактуры клиенту доходы/расходы привязываются к финпериоду автоматически

## Где смотреть финотчет
1. Меню *Отчетность* > *Финансовые отчеты*
2. Выбираем отчетный период и жмем кнопку *Открыть отчет*
![Рисунок. АРК: Online. Открытие финотчета](/assets/images/grid_tools/finreport_make.png)

## Как подготовить финотчет
1. Проверить, что доходы связаны с финпериодом [Аналитика / Отчетность. Контроль сумм клиенту](https://docs.arctl.ru/docs/analytics/fin_report_chek_cust/)
2. Проверить, что расходы связаны с финпериодом [Аналитика / Отчетность. Контроль расходов](https://docs.arctl.ru/docs/analytics/fin_report_chek_supp/)
3. Если в п.1 есть суммы без счетов-фактур, идем в отчеты по перевозкам и формируем недостающие счета-фактуры
4. Если в п.2 есть расходы без финпериода, идем в меню *Отчетность* > *Финансовые отчеты*, выбираем отчетный период и жмем *Привязать расходы*
![Рисунок. АРК: Online. Кнопка привязки расходов](/assets/images/grid_tools/finreport_attach_minus.png)

**Дожидаемся уведомления об успешном завершении продолжительного процесса!**

Аналогичная кнопка есть на панели инструментов вкладки "Расходы" в отчете по перевозке. Привязка происходит в рамках перевозки.
![Рисунок. АРК: Online. Кнопка привязки расходов](/assets/images/grid_tools/attach_minus_button.png)

> Если с помощью кнопки "Привязать расходы" расходы остались без установленного финпериода, значит система не смогла однозначно определить к какому счету-фактуре клиента относится расход. В этом случае привязка расхода к финпериоду производится **вручную** для каждого расхода.

**Важно!** После всех проверок рекомендуется закрыть период, поставив дату для финпериода.
