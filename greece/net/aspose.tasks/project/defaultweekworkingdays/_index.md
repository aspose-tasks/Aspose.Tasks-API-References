---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο της κλάσης WeekDayCollection που αντιπροσωπεύει μια συλλογή των προεπιλεγμένων εβδομαδιαίων ημερών εργασίας του έργου και των ωρών εργασίας"
type: docs
weight: 370
url: /el/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Λαμβάνει το αντικείμενο της κλάσης [`WeekDayCollection`](../../weekdaycollection/) που αντιπροσωπεύει μια συλλογή των προεπιλεγμένων εβδομαδιαίων ημερών εργασίας του έργου και των ωρών εργασίας.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Τιμή Επιστροφής

Το αντικείμενο της κλάσης [`WeekDayCollection`](../../weekdaycollection/) που περιέχει μια λίστα από αντικείμενα [`WeekDay`](../../weekday/).

## Παρατηρήσεις

Τα δεδομένα περιέχονται μόνο σε αρχεία mpp (όχι σε xml).

## Παραδείγματα

Δείχνει πώς να λάβετε την προεπιλεγμένη εβδομαδιαία ημέρα εργασίας.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Δείτε επίσης

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


