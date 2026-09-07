---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία"
type: docs
weight: 190
url: /el/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | DateTime | η ημερομηνία για τον υπολογισμό του τέλους της προηγούμενης εργασιακής ημέρας. |

### Τιμή Επιστροφής

Το τέλος του τέλους της προηγούμενης εργασιακής ημέρας.

## Παραδείγματα

Δείχνει πώς να λάβετε το τέλος της προηγούμενης εργάσιμης ημέρας χρησιμοποιώντας ένα ημερολόγιο.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε το τέλος της προηγούμενης εργάσιμης ημέρας
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 Απριλίου 2020 18:00 μ.μ. θα εκτυπωθεί
Console.WriteLine(previousWorkingDayEnd);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


