---
title: "Calendar.GetWorkingHours"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Возвращает WorkUnit, Start, Finish и Duration рабочих часов для указанного интервала даты и времени."
type: docs
weight: 220
url: /ru/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Возвращает WorkUnit — начало, конец и продолжительность рабочих часов для указанного интервала даты и времени.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала интервала. |
| завершение | DateTime | Дата завершения интервала. |

### Возвращаемое значение

Экземпляр класса [`WorkUnit`](../../workunit/), содержащий начало, конец и продолжительность рабочих часов.

## Примеры

Показывает, как получить рабочие часы для конкретных дат.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить рабочие часы для конкретной даты
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// Будет выведено 16 часов
Console.WriteLine(workUnit.WorkingHours);
```

### См. также

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Возвращает количество рабочих часов на указанную дату.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dt | DateTime | Дата, для которой нужно получить рабочие часы. |

### Возвращаемое значение

Рабочие часы на указанную дату.

## Примеры

Показывает, как получить рабочие часы для конкретной даты.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить рабочие часы для конкретной даты
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// Будут выведены 8 часов
Console.WriteLine(workingHours.Hours);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


