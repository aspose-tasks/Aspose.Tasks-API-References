---
title: "Απαρίθμηση MonthItemType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.MonthItemType. Καθορίζει το στοιχείο μήνα για το οποίο προγραμματίζεται μια επανάληψη εξαίρεσης"
type: docs
weight: 1050
url: /el/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Καθορίζει το στοιχείο μήνα για το οποίο προγραμματίζεται μια εξαίρεση επανάληψης.

```csharp
public enum MonthItemType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει μη καθορισμένο τύπο στοιχείου μήνα. |
| Day | `0` | Δείχνει τύπο στοιχείου μήνα Ημέρα. |
| Weekday | `1` | Δείχνει τύπο στοιχείου μήνα Εργάσιμη ημέρα. |
| WeekendDay | `2` | Δείχνει τύπο στοιχείου μήνα Σαββατοκύριακο. |
| Sunday | `3` | Δείχνει τύπο στοιχείου μήνα Κυριακή. |
| Monday | `4` | Δείχνει τύπο στοιχείου μήνα Δευτέρα. |
| Tuesday | `5` | Δείχνει τύπο στοιχείου μήνα Τρίτη. |
| Wednesday | `6` | Δείχνει τύπο στοιχείου μήνα Τετάρτη. |
| Thursday | `7` | Δείχνει τύπο στοιχείου μήνα Πέμπτη. |
| Friday | `8` | Δείχνει τύπο στοιχείου μήνα Παρασκευή. |
| Saturday | `9` | Δείχνει τύπο στοιχείου μήνα Σάββατο. |

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


