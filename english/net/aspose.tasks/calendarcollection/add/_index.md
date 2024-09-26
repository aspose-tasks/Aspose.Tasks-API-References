---
title: CalendarCollection.Add
second_title: Aspose.Tasks for .NET API Reference
description: CalendarCollection method. Adds a new base calendar to this CalendarCollection object and returns added calendar
type: docs
weight: 20
url: /net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Adds a new base calendar to this CalendarCollection object and returns added calendar.

```csharp
public Calendar Add(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Calendar name. |

### Return Value

Added [`Calendar`](../../calendar/) object.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Thrown when calendar name is null. |

## Examples

Shows how to make a standard calendar.

```csharp
var project = new Project();

// Define a calendar and make it standard
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Adds a new calendar with specified base calendar to this CalendarCollection object and returns added calendar.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Specified name. |
| baseCalendar | Calendar | Specified base calendar. |

### Return Value

Added [`Calendar`](../../calendar/) object.

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


