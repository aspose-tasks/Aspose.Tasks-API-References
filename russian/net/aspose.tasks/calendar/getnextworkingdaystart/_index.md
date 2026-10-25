---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Вычисляет начало следующего рабочего дня для указанной даты"
type: docs
weight: 180
url: /ru/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Вычисляет начало следующего рабочего дня для указанной даты.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| дата | DateTime | Дата, для которой требуется получить начало следующего рабочего дня. |

### Возвращаемое значение

Дата и время начала следующего рабочего дня.

## Примеры

Показывает, как получить начало следующего рабочего дня, используя календарь.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить начало следующего рабочего дня (выходные пропускаются)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 апреля 2020 г. 9:00 будет выведено
Console.WriteLine(nextWorkingDayStart);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


