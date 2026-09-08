---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ICalendar. Вычисляет дату и время завершения задачи из её частей даты начала и продолжительности работы."
type: docs
weight: 50
url: /ru/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Вычисляет дату и время завершения задачи на основе её даты начала, разбитых частей и длительности работы.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| задача | Задача | Задача, для которой вычисляется дата завершения. |
| продолжительность | TimeSpan | Продолжительность для вычисления. |

### Возвращаемое значение

Дата завершения задачи для заданных даты начала и продолжительности.

## Примечания

Возвращает DateTime.MinValue, если задача является сводной, null или её дата начала не установлена.

### См. также

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


