---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю"
type: docs
weight: 160
url: /ru/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала. |
| работа | Продолжительность | Продолжительность работы. |

### Возвращаемое значение

Дата завершения.

## Примеры

Показывает, как вычислить дату завершения по дате начала и объёму работы, используя экземпляр календаря.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// вычислить дату завершения с использованием стандартного календаря
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### См. также

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала. |
| работа | TimeSpan | Продолжительность работы. |

### Возвращаемое значение

Дата завершения.

## Примеры

Показывает, как вычислить дату завершения по дате начала и работе (в виде временного интервала), используя экземпляр календаря.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// вычислить дату завершения с использованием стандартного календаря
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


