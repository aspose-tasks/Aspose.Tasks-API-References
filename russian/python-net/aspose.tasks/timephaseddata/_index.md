---
title: "TimephasedData"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 1270
url: /ru/python-net/aspose.tasks/timephaseddata/
---

## TimephasedData class

Представляет данные, разбитые по времени.

Тип TimephasedData раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| TimephasedData() | Инициализирует новый экземпляр класса [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/). |
## Свойства
| Имя | Описание |
| :- | :- |
| value_to_units | Получает экземпляр float, представляющий строковое значение этого объекта для данных, фазированных по единицам. |
| uid | Получает или задает уникальный идентификатор данных, фазированных по времени |
| начало | Получает или задает дату начала периода данных, фазированных по времени. |
| finish | Получает или задает дату окончания периода данных, фазированных по времени. |
| unit | Получает или задает единицу времени периода данных, фазированных по времени. |
| timephased_data_type | Получает или задает тип данных, фазированных по времени. |
| value | Получает или задает значение за единицу времени для периода данных с фазированием по времени. |
| value_to_duration | Получает экземпляр datetime, который представляет строковое значение этого объекта. |
| value_to_cost | Получает экземпляр float, который представляет строковое значение этого объекта. |
## Методы
| Имя | Описание |
| :- | :- |
| create_cost_timephased(uid, start, finish, value, time_unit, type) |  |
| create_cost_timephased(uid, start, finish, value, type) |  |
| create_work_timephased(uid, start, finish, value, time_unit, type) | Создает и инициализирует новый экземпляр класса [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) для данных с фазированием по времени, основанных на работе. |
| create_unit_timephased(uid, start, finish, units, type) | Создает и инициализирует новый экземпляр класса [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) для данных с фазированием по времени, основанных на единицах, назначения материального ресурса. |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

