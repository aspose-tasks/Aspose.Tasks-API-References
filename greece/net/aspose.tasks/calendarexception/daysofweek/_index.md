---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException ιδιότητα. Λαμβάνει το DayTypeCollection για αυτό το αντικείμενο. Οι ημέρες της εβδομάδας στις οποίες η εξαίρεση είναι έγκυρη"
type: docs
weight: 20
url: /el/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Λαμβάνει το DayTypeCollection για αυτό το αντικείμενο. Οι ημέρες της εβδομάδας στις οποίες η εξαίρεση είναι έγκυρη.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε εξαίρεση ημερολογίου ανά ημέρα της εβδομάδας.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// δημιουργήστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// δημιουργήστε εξαίρεση ημερολογίου για κάθε Παρασκευή
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// ελέγξτε ότι η Παρασκευή είναι εξαίρεση
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// προσθέστε την εξαίρεση στο ημερολόγιο
calendar.Exceptions.Add(exception);
```

### Δείτε επίσης

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


