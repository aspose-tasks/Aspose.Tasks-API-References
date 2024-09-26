---
title: Calendar.Delete
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Removes calendar from project
type: docs
weight: 130
url: /net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Removes calendar from project.

```csharp
public void Delete()
```

## Examples

Shows how to delete a calendar from a project.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// get the calendar by name
var calendar = project.Calendars.GetByName("Broken Calendar");

// delete the calendar
calendar.Delete();
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


