---
title: Calendar.GetWorkingHours
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Return WorkUnit  Start Finish and Duration of working hours for the specified date time interval
type: docs
weight: 220
url: /net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start date of the interval. |
| finish | DateTime | Finish date of the interval. |

### Return Value

Instance of [`WorkUnit`](../../workunit/) class containing Start, Finish and Duration of working hours.

## Examples

Shows how to get working hours for specific dates.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get working hours for specific date
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 hours will be printed
Console.WriteLine(workUnit.WorkingHours);
```

### See Also

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Returns the amount of working hours at the specified date.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dt | DateTime | The date to get working hours for. |

### Return Value

Working hours at the specified date.

## Examples

Shows how to get working hours for a specific date.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get working hours for specific date
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 hours will be printed
Console.WriteLine(workingHours.Hours);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


