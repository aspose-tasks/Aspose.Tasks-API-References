---
title: ResourceAssignment.MakeTPs
second_title: Справочник по Aspose.Tasks для .NET API
description: ResourceAssignment метод. Генерирует список поэтапных данных по времени.
type: docs
weight: 730
url: /ru/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Генерирует список поэтапных данных по времени.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Указанная дата начала. |
| time | TimeSpan | Указанное время работы. |
| calendar | Calendar | Указанный рабочий календарь. |
| list | List`1 | Список поэтапных по времени данных. |
| isWorking | Boolean | Указанный флаг, указывающий, работают ли поэтапные данные. |
| type | Int32 | Указанный поэтапный тип данных. |

### Возвращаемое значение

Максимальная дата из списка или дата начала, если список пуст.

### Смотрите также

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* пространство имен [Aspose.Tasks](../../resourceassignment/)
* сборка [Aspose.Tasks](../../../)


