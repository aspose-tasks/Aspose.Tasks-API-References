---
title: Calendar.GetFinishDateByStartAndWork
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Calculates the date when the specified amount of work time will pass according to the calendar
type: docs
weight: 150
url: /net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Calculates the date when the specified amount of work time will pass according to the calendar.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start date. |
| work | Duration | Work duration. |

### Return Value

Finish date.

## Examples

Shows how to calculate a finish date by start date and work using a calendar instance.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calculate finish date by using a standard calendar
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### See Also

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Calculates the date when the specified amount of work time will pass according to the calendar.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start date. |
| work | TimeSpan | Work duration. |

### Return Value

Finish date.

## Examples

Shows how to calculate a finish date by start date and work (as a time span) using a calendar instance.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calculate finish date by using a standard calendar
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


