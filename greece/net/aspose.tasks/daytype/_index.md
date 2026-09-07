---
title: "Απαρίθμηση DayType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.DayType απαρίθμηση. Καθορίζει την ημέρα της εβδομάδας"
type: docs
weight: 450
url: /el/net/aspose.tasks/daytype/
---
## DayType enumeration

Καθορίζει την ημέρα της εβδομάδας.

```csharp
public enum DayType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Exception | `0` | Δείχνει τύπο ημέρας Εξαίρεση. |
| Sunday | `1` | Δείχνει τύπο ημέρας Κυριακή. |
| Monday | `2` | Δείχνει τύπο ημέρας Δευτέρα. |
| Tuesday | `3` | Δείχνει τύπο ημέρας Τρίτη. |
| Wednesday | `4` | Δείχνει τύπο ημέρας Τετάρτη. |
| Thursday | `5` | Δείχνει τύπο ημέρας Πέμπτη. |
| Friday | `6` | Δείχνει τύπο ημέρας Παρασκευή. |
| Saturday | `7` | Δείχνει τύπο ημέρας Σάββατο. |

## Παραδείγματα

Δείχνει πώς να ορίσετε ένα νέο ημερολόγιο, να προσθέσετε ημέρες της εβδομάδας σε αυτό και να ορίσετε ώρες εργασίας για τις ημέρες.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Προσθέστε εργάσιμες ημέρες από τη Δευτέρα έως την Πέμπτη με προεπιλεγμένα ωράρια
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Ορίστε την Παρασκευή ως σύντομη εργάσιμη ημέρα
var weekDay = new WeekDay(DayType.Friday);

// Ορίζει χρόνο εργασίας. Μόνο το τμήμα ώρας του DateTime είναι σημαντικό.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// εργασία με το έργο...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


