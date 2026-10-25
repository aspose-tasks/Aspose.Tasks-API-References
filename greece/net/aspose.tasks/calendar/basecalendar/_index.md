---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει ή ορίζει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Ισχύει μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο"
type: docs
weight: 40
url: /el/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Λαμβάνει ή ορίζει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Ισχύει μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με ένα βασικό ημερολόγιο του ημερολογίου του πόρου.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Προσθέστε τυπικό ημερολόγιο και αναθέστε το σε πόρο
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Εμφάνιση ονόματος βασικού ημερολογίου για όλους τους πόρους
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


