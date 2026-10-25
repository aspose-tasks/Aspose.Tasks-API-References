---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Возвращает дату начала на основе указанной даты завершения и продолжительности"
type: docs
weight: 200
url: /ru/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Возвращает дату начала, исходя из указанной даты завершения и длительности.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| завершение | DateTime | Указанная дата завершения. |
| продолжительность | Продолжительность | Указанная продолжительность. |

### Возвращаемое значение

Вычисленная дата начала.

## Примеры

Показывает, как получить дату начала по дате завершения и продолжительности.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить дату начала по дате завершения и продолжительности
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 апреля 2020 г. 9:00 будет выведено
Console.WriteLine(startDate);
```

### См. также

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Возвращает дату начала, исходя из указанной даты завершения и длительности.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| завершение | DateTime | Указанная дата завершения. |
| продолжительность | TimeSpan | Указанная продолжительность. |

### Возвращаемое значение

Вычисленная дата начала.

## Примеры

Показывает, как получить дату начала по дате завершения и продолжительности (в виде временного интервала).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить дату начала по дате завершения и продолжительности
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 апреля 2020 г. 9:00 будет выведено
Console.WriteLine(startDate);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


