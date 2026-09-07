---
title: "Duration.Convert"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Μετατρέπει το αντικείμενο Duration σε άλλη διάρκεια με καθορισμένες μονάδες χρόνου"
type: docs
weight: 70
url: /el/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Μετατρέπει το αντικείμενο Duration σε άλλη διάρκεια με καθορισμένες μονάδες χρόνου.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| timeUnitType | TimeUnitType | ο καθορισμένος τύπος μονάδας χρόνου. |

### Τιμή Επιστροφής

επιστρέφει νέα διάρκεια με τον καθορισμένο τύπο μονάδας.

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

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


