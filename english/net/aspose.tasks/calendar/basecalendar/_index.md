---
title: Calendar.BaseCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets or sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar
type: docs
weight: 40
url: /net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Gets or sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Examples

Shows how to work with a base calendar of the resource's calendar.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Add standard calendar and assign to resource
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Display base calendar name for all resources
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


