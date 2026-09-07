---
title: "Calendar.Uid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό του ημερολογίου"
type: docs
weight: 110
url: /el/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό του ημερολογίου.

```csharp
public int Uid { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες ημερολογίου.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Ανάκτηση Πληροφοριών Ημερολογίων
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


