---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Επιστρέφει WorkingTimeCollection των ωρών εργασίας για την καθορισμένη ημερομηνία"
type: docs
weight: 240
url: /el/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Επιστρέφει [`WorkingTimeCollection`](../../workingtimecollection/) των εργάσιμων χρόνων για την καθορισμένη ημερομηνία.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | Η ημερομηνία για την οποία θα ληφθούν οι ώρες εργασίας. |

### Τιμή Επιστροφής

Συλλογή αντικειμένων [`WorkingTime`](../../workingtime/).

## Παραδείγματα

Δείχνει πώς να λάβετε ώρες εργασίας για μια συγκεκριμένη ημερομηνία.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ώρες εργασίας για συγκεκριμένη ημερομηνία
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 ώρες θα εκτυπωθούν
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Δείτε επίσης

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


