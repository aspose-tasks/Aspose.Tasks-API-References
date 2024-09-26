---
title: Calendar.Exceptions
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar
type: docs
weight: 50
url: /net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Examples

Shows how to retrieve info about calendar exceptions.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Iterate over calendars
foreach (var calendar in project.Calendars)
{
    // Access calendar exceptions
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### See Also

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


