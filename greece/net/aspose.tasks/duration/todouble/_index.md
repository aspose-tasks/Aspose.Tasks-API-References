---
title: "Duration.ToDouble"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Μετατρέπει το αντικείμενο Duration σε τιμή Double"
type: docs
weight: 110
url: /el/net/aspose.tasks/duration/todouble/
---
## Duration.ToDouble method

Μετατρέπει το αντικείμενο Duration σε τιμή Double.

```csharp
public double ToDouble()
```

### Τιμή Επιστροφής

Μετατρεπόμενη τιμή.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


