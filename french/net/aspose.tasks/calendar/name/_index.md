---
title: "Calendar.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient ou définit le nom du calendrier"
type: docs
weight: 90
url: /fr/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Obtient ou définit le nom du calendrier.

```csharp
public string Name { get; set; }
```

## Exemples

Montre comment récupérer les informations du calendrier.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Récupérer les informations des calendriers
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

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


