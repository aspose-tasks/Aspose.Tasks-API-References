---
title: Rsc.Calendar
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The calendar of a resource
type: docs
weight: 190
url: /net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

The calendar of a resource.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Examples

Shows how to get/set a resource calendar.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Add standard calendar and assign to resource
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Display base calendar name for all resources
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


