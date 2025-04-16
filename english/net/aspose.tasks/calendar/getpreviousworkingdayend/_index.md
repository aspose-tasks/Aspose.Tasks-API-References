---
title: Calendar.GetPreviousWorkingDayEnd
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Calculates the end of the previous working date from the specified date
type: docs
weight: 180
url: /net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Calculates the end of the previous working date from the specified date.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parameter | Type | Description |
| --- | --- | --- |
| date | DateTime | the date to calculate the previous working day end. |

### Return Value

The end of the previous working day end

## Examples

Shows how to get a previous working day end by using a calendar.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get previous working day end
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 April 2020 18:00 PM will be printed
Console.WriteLine(previousWorkingDayEnd);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


