---
title: Calendar.IsBaselineCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets or sets a value indicating whether the calendar is a baseline calendar
type: docs
weight: 80
url: /net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Gets or sets a value indicating whether the calendar is a baseline calendar.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Examples

Shows how to check whether a calendar is baseline calendar or not.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


