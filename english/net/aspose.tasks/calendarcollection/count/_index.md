---
title: Count
second_title: Aspose.Tasks for .NET API Reference
description: Gets the number of objects contained in this CalendarCollectionaspose.tasks/calendarcollection object.
type: docs
weight: 10
url: /net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Gets the number of objects contained in this [`CalendarCollection`](../../calendarcollection) object.

```csharp
public int Count { get; }
```

### Examples

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

* class [CalendarCollection](../../calendarcollection)
* namespace [Aspose.Tasks](../../calendarcollection)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
