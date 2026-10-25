---
title: "Enum TimeUnitType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TimeUnitType enum. Καθορίζει τον τύπο μιας μονάδας χρόνου"
type: docs
weight: 2570
url: /el/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Καθορίζει τον τύπο μιας μονάδας χρόνου.

```csharp
public enum TimeUnitType : sbyte
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει ότι η τιμή Undefined σημαίνει ότι το πεδίο δεν ορίστηκε στο αρχικό αρχείο έργου. |
| Minute | `0` | Δείχνει τύπο μονάδας χρόνου λεπτό. |
| ElapsedMinute | `1` | Δείχνει τύπο μονάδας χρόνου περασμένο λεπτό. |
| Hour | `2` | Δείχνει τύπο μονάδας χρόνου ώρα. |
| ElapsedHour | `3` | Δείχνει τύπο μονάδας χρόνου περασμένη ώρα. |
| Day | `4` | Δείχνει τύπο μονάδας χρόνου ημέρα. |
| ElapsedDay | `5` | Δείχνει τύπο μονάδας χρόνου περασμένη ημέρα. |
| Week | `6` | Δείχνει τύπο μονάδας χρόνου εβδομάδα. |
| ElapsedWeek | `7` | Δείχνει τύπο μονάδας χρόνου περασμένη εβδομάδα. |
| Month | `8` | Δείχνει τύπο μονάδας χρόνου μήνας. |
| ElapsedMonth | `9` | Δείχνει τύπο μονάδας χρόνου περασμένος μήνας. |
| Percent | `10` | Δείχνει τύπο μονάδας χρόνου ποσοστό. |
| ElapsedPercent | `11` | Δείχνει τύπο μονάδας χρόνου περασμένο ποσοστό. |
| Null | `12` | Δείχνει τύπο μονάδας χρόνου Null. |
| MinuteEstimated | `13` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενο λεπτό. |
| ElapsedMinuteEstimated | `14` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενο περασμένο λεπτό. |
| HourEstimated | `15` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη ώρα. |
| ElapsedHourEstimated | `16` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη περασμένη ώρα. |
| DayEstimated | `17` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη ημέρα. |
| ElapsedDayEstimated | `18` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη περασμένη ημέρα. |
| WeekEstimated | `19` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη εβδομάδα. |
| ElapsedWeekEstimated | `20` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενη περασμένη εβδομάδα. |
| MonthEstimated | `21` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενος μήνας. |
| ElapsedMonthEstimated | `22` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενος περασμένος μήνας. |
| PercentEstimated | `23` | Δείχνει τύπο μονάδας χρόνου εκτιμώμενο ποσοστό. |
| ElapsedPercentEstimated | `24` | Δείχνει τον τύπο μονάδας χρόνου εκτιμώμενου ποσοστού που έχει παρέλθει. |
| Year | `25` | Δείχνει τον τύπο μονάδας χρόνου Έτος. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Εμφανίζει πώς να μετατρέψετε μια διάρκεια σε διαφορετικούς τύπους μονάδων χρόνου.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Αποκτήστε μια εργασία για να υπολογίσετε τη διάρκεια της σε διαφορετικές μορφές
var task = project.RootTask.Children.GetById(1);

// Αποκτήστε τη διάρκεια σε Λεπτά, Ημέρες, Ώρες, Εβδομάδες και Μήνες
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


