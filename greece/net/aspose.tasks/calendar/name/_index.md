---
title: "Calendar.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει ή ορίζει το όνομα του ημερολογίου."
type: docs
weight: 90
url: /el/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Λαμβάνει ή ορίζει το όνομα του ημερολογίου.

```csharp
public string Name { get; set; }
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


