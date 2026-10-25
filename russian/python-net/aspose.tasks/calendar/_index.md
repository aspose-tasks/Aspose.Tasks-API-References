---
title: "Calendar"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 140
url: /ru/python-net/aspose.tasks/calendar/
---

## Calendar class

Представляет календарь, используемый в проекте.

Тип Calendar раскрывает следующие члены:
## Свойства
| Имя | Описание |
| :- | :- |
| name | Получает или задает название календаря. |
| uid | Получает или задает уникальный идентификатор календаря. |
| week_days | Получает WeekDaysCollection для этого календаря.<br/>            Коллекция дней недели, определяющая календарь. |
| exceptions | Получает объект CalendarExceptionCollection.<br/>            Коллекция исключений, связанных с календарем. |
| work_weeks | Получает объект WorkWeekCollections.<br/>            Коллекция рабочих недель, связанных с календарем. |
| is_base_calendar | Получает значение, указывающее, является ли календарь базовым. |
| base_calendar | Получает или задает базовый календарь, от которого зависит этот календарь.<br/>            Применяется только если календарь не является базовым. |
| is_baseline_calendar | Получает или задает значение, указывающее, является ли календарь календарем базовой линии. |
| guid | Получает Guid календаря. |
| primavera_properties | Получает объект, содержащий свойства, специфичные для Primavera, для календаря, считанного из форматов Primavera. |
## Методы
| Имя | Описание |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Возвращает дату начала, основанную на указанной дате завершения и длительности. |
| get_start_date_from_finish_and_duration(finish, duration) | Возвращает дату начала, основанную на указанной дате завершения и длительности. |
| get_working_hours(start, finish) | Возвращает WorkUnit — начало, окончание и продолжительность рабочих часов для указанного временного интервала. |
| get_working_hours(dt) | Возвращает WorkUnit — начало, окончание и продолжительность рабочих часов для указанного временного интервала. |
| get_finish_date_by_start_and_work(start, work) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| get_finish_date_by_start_and_work(start, work) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| get_intersection_calendar(calendar1, calendar2) | Получает экземпляр [ICalendar](/tasks/python-net/aspose.tasks/icalendar/), который можно использовать для выполнения вычислений пересечения графиков работы двух календарей. |
| make_standard_calendar(calendar) | Создает стандартный календарь по умолчанию. |
| make_24_hour_calendar(calendar) | Преобразует заданный Calendar в 24-часовой календарь.<br/>            24-часовой календарь — это календарь, в котором каждый день недели работает круглосуточно. |
| make_night_shift_calendar(calendar) | Преобразует заданный Calendar в ночной сменный календарь. |
| delete() | Удаляет календарь из проекта. |
| is_day_working(dt) | Определяет, является ли указанный день рабочим согласно календарю. |
| get_working_hours_time_span(start, finish) | Возвращает количество рабочих часов между указанными датами. |
| get_task_finish_date_from_duration(task, duration) | Вычисляет дату и время завершения задачи исходя из её даты начала, разбитых частей и продолжительности работы. |
| get_working_times(dt) | Возвращает [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) рабочих времён для указанной даты. |
| get_previous_working_day_end(date) | Вычисляет конец предыдущего рабочего дня от указанной даты. |
| get_next_working_day_start(date) | Вычисляет начало следующего рабочего дня для указанной даты. |
| get_work_start(date) | Вычисляет начало следующего рабочего периода, начиная с указанной даты и времени. |
| is_empty() | Возвращает, не имеет ли календарь определённых рабочих часов. |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

