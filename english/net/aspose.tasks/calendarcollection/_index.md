---
title: Class CalendarCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CalendarCollection class. Represents a collection of Calendar objects
type: docs
weight: 240
url: /net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Represents a collection of [`Calendar`](../calendar/) objects.

```csharp
public class CalendarCollection : IList<Calendar>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Gets the number of objects contained in this `CalendarCollection` object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Adds a new base calendar to this CalendarCollection object and returns added calendar. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Adds a new calendar with specified base calendar to this CalendarCollection object and returns added calendar. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Returns a calendar with the specified name. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Returns a calendar with the specified UID. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Removes Calendar from Project CalendarCollection. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Converts the CalendarCollection object to a list of [`Calendar`](../calendar/) objects. |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


