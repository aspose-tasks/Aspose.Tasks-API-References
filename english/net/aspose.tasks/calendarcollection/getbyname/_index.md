---
title: CalendarCollection.GetByName
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Returns a calendar with the specified name
type: docs
weight: 30
url: /net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Returns a calendar with the specified name.

```csharp
public Calendar GetByName(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Name of a calendar. |

### Return Value

If found returns calendar with a specified name else returns null.

## Examples

Shows how to get calendars by name or by id.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### See Also

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


