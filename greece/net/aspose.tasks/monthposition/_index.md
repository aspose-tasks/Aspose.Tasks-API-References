---
title: "Απαρίθμηση MonthPosition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.MonthPosition. Καθορίζει τη θέση ενός στοιχείου μήνα μέσα σε ένα μήνα"
type: docs
weight: 1070
url: /el/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Καθορίζει τη θέση ενός στοιχείου μήνα μέσα σε έναν μήνα.

```csharp
public enum MonthPosition
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει ακαθόριστη θέση μήνα. |
| First | `0` | Δείχνει την πρώτη θέση μήνα. |
| Second | `1` | Δείχνει τη δεύτερη θέση μήνα. |
| Third | `2` | Δείχνει την τρίτη θέση μήνα. |
| Fourth | `3` | Δείχνει τη θέση του τέταρτου μήνα. |
| Last | `4` | Δείχνει τη θέση του τελευταίου μήνα. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


