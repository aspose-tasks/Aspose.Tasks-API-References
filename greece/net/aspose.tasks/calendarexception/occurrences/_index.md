---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException ιδιότητα. Λαμβάνει ή ορίζει τον αριθμό των εμφανίσεων για τις οποίες η εξαίρεση ημερολογίου είναι έγκυρη"
type: docs
weight: 110
url: /el/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Λαμβάνει ή ορίζει τον αριθμό των επαναλήψεων για τις οποίες η εξαίρεση του ημερολογίου είναι έγκυρη.

```csharp
public int Occurrences { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια εξαίρεση ημερολογίου με εμφανίσεις.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Ορίστε εξαίρεση και καθορίστε εμφανίσεις
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Προσθέστε εξαίρεση στο ημερολόγιο
calendar.Exceptions.Add(exception);
```

### Δείτε επίσης

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


