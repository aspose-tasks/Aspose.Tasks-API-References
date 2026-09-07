---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ημερολόγιο ενός πόρου"
type: docs
weight: 190
url: /el/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Το ημερολόγιο ενός πόρου.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Παραδείγματα

Δείχνει πώς να λάβετε/ορίσετε ένα ημερολόγιο πόρου.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Προσθέστε τυπικό ημερολόγιο και αναθέστε το σε πόρο
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Εμφάνιση ονόματος βασικού ημερολογίου για όλους τους πόρους
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


