---
title: CalendarCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Returns an enumerator for this collection
type: docs
weight: 50
url: /net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Return Value

an enumerator for this collection.

## Examples

Shows how to add new calendars.

```csharp
var project = new Project();

// new calendars can be added to a project's calendar collection by using the collection's Add overloads.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### See Also

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


