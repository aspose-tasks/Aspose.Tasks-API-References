---
title: "Rsc.Calendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le calendrier d'une ressource"
type: docs
weight: 190
url: /fr/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Le calendrier d'une ressource.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Exemples

Montre comment obtenir/mettre à jour le calendrier d'une ressource.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Ajouter un calendrier standard et l'assigner à la ressource
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Afficher le nom du calendrier de base pour toutes les ressources
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


