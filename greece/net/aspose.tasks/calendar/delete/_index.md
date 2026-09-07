---
title: "Calendar.Delete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Αφαιρεί το ημερολόγιο από το έργο"
type: docs
weight: 140
url: /el/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Αφαιρεί το ημερολόγιο από το έργο.

```csharp
public void Delete()
```

## Παραδείγματα

Δείχνει πώς να διαγράψετε ένα ημερολόγιο από ένα έργο.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// Λάβετε το ημερολόγιο με όνομα
var calendar = project.Calendars.GetByName("Broken Calendar");

// διαγράψτε το ημερολόγιο
calendar.Delete();
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


