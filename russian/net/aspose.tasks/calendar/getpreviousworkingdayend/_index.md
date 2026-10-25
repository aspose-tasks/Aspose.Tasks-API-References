---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Вычисляет конец предыдущего рабочего дня, исходя из указанной даты"
type: docs
weight: 190
url: /ru/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Вычисляет конец предыдущего рабочего дня относительно указанной даты.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| дата | DateTime | Дата, для которой вычисляется конец предыдущего рабочего дня. |

### Возвращаемое значение

Конец предыдущего рабочего дня.

## Примеры

Показывает, как получить конец предыдущего рабочего дня, используя календарь.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить конец предыдущего рабочего дня
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 апреля 2020 18:00 PM будет выведено
Console.WriteLine(previousWorkingDayEnd);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


