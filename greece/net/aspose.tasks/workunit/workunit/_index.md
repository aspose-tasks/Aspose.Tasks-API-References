---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής WorkUnit. Αρχικοποιεί μια νέα παρουσία της κλάσης WorkUnit. Δημιουργεί νέο αντικείμενο WorkUnit με τις καθορισμένες ημερομηνίες From και To"
type: docs
weight: 10
url: /el/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`WorkUnit`](../). Δημιουργεί νέο αντικείμενο WorkUnit με τις καθορισμένες ημερομηνίες From και To.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| από | DateTime | Ημερομηνία έναρξης των ωρών εργασίας. |
| σε | DateTime | Ημερομηνία λήξης των ωρών εργασίας. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με πληροφορίες μονάδας εργασίας.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ώρες εργασίας για συγκεκριμένη ημερομηνία
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Δείτε επίσης

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


