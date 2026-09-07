---
title: "CalendarException.Period"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException ιδιότητα. Λαμβάνει ή ορίζει την περίοδο επανάληψης για την εξαίρεση."
type: docs
weight: 130
url: /el/net/aspose.tasks/calendarexception/period/
---
## CalendarException.Period property

Λαμβάνει ή ορίζει την περίοδο επανάληψης για την εξαίρεση.

```csharp
public int Period { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε εξαίρεση ημερολογίου ανά ημέρα του μήνα.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// δημιουργήστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// δημιουργήστε εξαίρεση ημερολογίου για κάθε Παρασκευή
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// ελέγξτε ότι η Παρασκευή είναι εξαίρεση
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// προσθέστε την εξαίρεση στο ημερολόγιο
calendar.Exceptions.Add(exception);
```

### Δείτε επίσης

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


