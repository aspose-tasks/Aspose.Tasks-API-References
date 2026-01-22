---
title: Calendar.PrimaveraProperties
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets an object containing Primaveraspecific properties for a calendar read from Primavera formats
type: docs
weight: 100
url: /net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Gets an object containing Primavera-specific properties for a calendar read from Primavera formats.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Examples

Shows how to read a project from a Primavera file and examine calendar's Primavera-specific properties.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Returns project with special Uid
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### See Also

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


