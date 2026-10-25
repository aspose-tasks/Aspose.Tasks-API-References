---
title: "WorkUnit.From"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα WorkUnit. Λαμβάνει ή ορίζει την ημερομηνία From"
type: docs
weight: 20
url: /el/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Λαμβάνει ή ορίζει την ημερομηνία From.

```csharp
public DateTime From { get; set; }
```

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


