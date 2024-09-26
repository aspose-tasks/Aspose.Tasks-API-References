---
title: CalendarCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Converts the CalendarCollection object to a list of Calendar objects
type: docs
weight: 70
url: /net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Converts the CalendarCollection object to a list of [`Calendar`](../../calendar/) objects.

```csharp
public List<Calendar> ToList()
```

### Return Value

List of [`Calendar`](../../calendar/) objects.

## Examples

Shows how to iterate over calendar collection.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### See Also

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


