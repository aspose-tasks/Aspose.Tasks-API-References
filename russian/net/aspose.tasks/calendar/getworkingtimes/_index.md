---
title: "Calendar.GetWorkingTimes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Возвращает WorkingTimeCollection рабочих периодов для указанной даты"
type: docs
weight: 240
url: /ru/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Возвращает [`WorkingTimeCollection`](../../workingtimecollection/) рабочих периодов для указанной даты.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dt | DateTime | Дата, для которой нужно получить рабочие часы. |

### Возвращаемое значение

Коллекция экземпляров [`WorkingTime`](../../workingtime/).

## Примеры

Показывает, как получить рабочие периоды для конкретной даты.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить рабочие периоды для конкретной даты
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// Будет выведено 16 часов
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### См. также

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


