---
title: Calendar.Uid
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets or sets the unique identifier of the calendar
type: docs
weight: 110
url: /net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Gets or sets the unique identifier of the calendar.

```csharp
public int Uid { get; set; }
```

## Examples

Shows how to retrieve calendar info.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Retrieve Calendars Information
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


