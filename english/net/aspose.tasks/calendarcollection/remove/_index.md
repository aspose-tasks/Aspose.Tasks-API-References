---
title: CalendarCollection.Remove
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Removes Calendar from Project CalendarCollection
type: docs
weight: 60
url: /net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Removes Calendar from Project CalendarCollection.

```csharp
public bool Remove(Calendar item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | Calendar | The calendar to remove. |

### Return Value

If removed returns true, else returns false.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Thrown when calendar cannot be removed. |

## Examples

Shows how to replace a calendar in the collection.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// add new calendar
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


