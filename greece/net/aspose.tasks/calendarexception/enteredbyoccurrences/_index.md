---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "CalendarException ιδιότητα. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. False καθορίζει ότι η περιοχή επανάληψης ορίζεται με την εισαγωγή ημερομηνίας λήξης."
type: docs
weight: 40
url: /el/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού επαναλήψεων. False υποδεικνύει ότι η περιοχή επανάληψης ορίζεται με την εισαγωγή ημερομηνίας λήξης.

```csharp
public bool EnteredByOccurrences { get; set; }
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


