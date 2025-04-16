---
title: Calendar.GetNextWorkingDayStart
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Calculates next working day start for the specified date
type: docs
weight: 170
url: /net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Calculates next working day start for the specified date.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parameter | Type | Description |
| --- | --- | --- |
| date | DateTime | The date to get next working day start for. |

### Return Value

Next working day start DateTime.

## Examples

Shows how to get a next working day start by using a calendar.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get next working day start (weekend is skipped)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 April 2020 9:00 AM will be printed
Console.WriteLine(nextWorkingDayStart);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


