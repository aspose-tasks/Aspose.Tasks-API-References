---
title: "Απαρίθμηση CalendarExceptionType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.CalendarExceptionType. Καθορίζει τον τύπο εξαίρεσης του ημερολογίου."
type: docs
weight: 270
url: /el/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Καθορίζει τον τύπο εξαίρεσης ημερολογίου.

```csharp
public enum CalendarExceptionType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Daily | `0` | Δείχνει τύπο ημερήσιας εξαίρεσης. |
| YearlyByDay | `1` | Δείχνει ετήσια εξαίρεση κατά ημέρα του μήνα. |
| YearlyByPosition | `2` | Δείχνει ετήσια εξαίρεση κατά θέση. |
| MonthlyByDay | `3` | Δείχνει μηνιαία εξαίρεση κατά ημέρα του μήνα. |
| MonthlyByPosition | `4` | Δείχνει μηνιαία εξαίρεση κατά θέση. |
| Weekly | `5` | Υποδεικνύει τύπο εξαίρεσης εβδομαδιαίας. |
| ByDayCount | `6` | Υποδεικνύει τύπο εξαίρεσης κατά αριθμό ημερών. |
| ByWeekDayCount | `7` | Υποδεικνύει τύπο εξαίρεσης κατά αριθμό ημερών της εβδομάδας. |
| NoExceptionType | `8` | Υποδεικνύει τύπο χωρίς εξαίρεση. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


