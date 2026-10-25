---
title: "Calendar.BaseCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient ou définit le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base"
type: docs
weight: 40
url: /fr/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Obtient ou définit le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Exemples

Montre comment travailler avec le calendrier de base du calendrier de la ressource.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Ajouter un calendrier standard et l'assigner à la ressource
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Afficher le nom du calendrier de base pour toutes les ressources
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


