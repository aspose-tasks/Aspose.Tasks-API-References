---
title: Calendar.GetWorkingTimes
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Returns WorkingTimeCollection of working times for the specified date
type: docs
weight: 240
url: /net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Returns [`WorkingTimeCollection`](../../workingtimecollection/) of working times for the specified date.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dt | DateTime | The date to get working times for. |

### Return Value

Collection of [`WorkingTime`](../../workingtime/) instances.

## Examples

Shows how to get working times for a specific date.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get working times for specific date
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 hours will be printed
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### See Also

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


