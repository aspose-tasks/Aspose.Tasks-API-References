---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Справочник по Aspose.Tasks для .NET API
description: Calendar метод. Вычисляет дату и время окончания задачи исходя из даты ее начала разделенных частей и продолжительности.
type: docs
weight: 190
url: /ru/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Вычисляет дату и время окончания задачи, исходя из даты ее начала, разделенных частей и продолжительности.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| task | Task | Задача, для которой нужно получить дату окончания. |
| duration | TimeSpan | Продолжительность задачи для разделения. |

### Возвращаемое значение

Дата окончания задачи.

### Примечания

Возвращает DateTime.MinValue, если задача является сводной, нулевой или дата ее начала не задана.

### Смотрите также

* class [Task](../../task/)
* class [Calendar](../)
* пространство имен [Aspose.Tasks](../../calendar/)
* сборка [Aspose.Tasks](../../../)


