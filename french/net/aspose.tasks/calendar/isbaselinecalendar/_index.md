---
title: "Calendar.IsBaselineCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient ou définit une valeur indiquant si le calendrier est un calendrier de référence"
type: docs
weight: 80
url: /fr/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Obtient ou définit une valeur indiquant si le calendrier est un calendrier de référence.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Exemples

Montre comment vérifier si un calendrier est un calendrier de référence ou non.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


