---
title: CalendarCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection property. Gets the number of objects contained in this CalendarCollection object
type: docs
weight: 10
url: /net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Gets the number of objects contained in this [`CalendarCollection`](../) object.

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


