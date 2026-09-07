---
title: "Κλάση WorkUnit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.WorkUnit. Αντιπροσωπεύει ώρες εργασίας"
type: docs
weight: 3630
url: /el/net/aspose.tasks/workunit/
---
## WorkUnit class

Αντιπροσωπεύει ώρες εργασίας.

```csharp
public class WorkUnit
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `WorkUnit`. Δημιουργεί νέο αντικείμενο WorkUnit με τις καθορισμένες ημερομηνίες From και To. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Λαμβάνει ή ορίζει τη διάρκεια των ωρών εργασίας. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


