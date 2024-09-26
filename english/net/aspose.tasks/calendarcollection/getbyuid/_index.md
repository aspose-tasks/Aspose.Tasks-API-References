---
title: CalendarCollection.GetByUid
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Returns a calendar with the specified UID
type: docs
weight: 40
url: /net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Returns a calendar with the specified UID.

```csharp
public Calendar GetByUid(int uid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID of a calendar. |

### Return Value

Calendar with a specified UID.

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


