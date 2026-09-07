---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία"
type: docs
weight: 180
url: /el/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | DateTime | Η ημερομηνία για την οποία θα ληφθεί η έναρξη της επόμενης εργάσιμης ημέρας. |

### Τιμή Επιστροφής

DateTime έναρξης επόμενης εργάσιμης ημέρας.

## Παραδείγματα

Δείχνει πώς να λάβετε την έναρξη της επόμενης εργάσιμης ημέρας χρησιμοποιώντας ένα ημερολόγιο.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε την έναρξη της επόμενης εργάσιμης ημέρας (το Σαββατοκύριακο παραλείπεται)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 Απριλίου 2020 9:00 π.μ. θα εκτυπωθεί
Console.WriteLine(nextWorkingDayStart);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


