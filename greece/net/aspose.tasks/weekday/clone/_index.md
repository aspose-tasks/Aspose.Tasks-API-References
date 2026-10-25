---
title: "WeekDay.Clone"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "WeekDay μέθοδος. Επιστρέφει ένα βαθύ αντίγραφο της ημέρας της εβδομάδας"
type: docs
weight: 80
url: /el/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Επιστρέφει ένα βαθύ αντίγραφο της ημέρας της εβδομάδας.

```csharp
public WeekDay Clone()
```

### Τιμή Επιστροφής

Επιστρέφει το βαθύ αντίγραφο της ημέρας της εβδομάδας.

## Παραδείγματα

Δείχνει πώς να κλωνοποιήσετε μια ημέρα της εβδομάδας.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// δημιουργήστε ένα βαθύ αντίγραφο ημέρας της εβδομάδας
var weekDay2 = weekDay1.Clone();

// η ισότητα των ημερολογίων ελέγχεται έναντι των ιδιοτήτων της ημέρας της εβδομάδας:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Δείτε επίσης

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


