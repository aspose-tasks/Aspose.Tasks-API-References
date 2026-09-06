---
title: "CalendarCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Supprime le calendrier du CalendarCollection du projet"
type: docs
weight: 60
url: /fr/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Supprime Calendar du CalendarCollection du projet.

```csharp
public bool Remove(Calendar item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | Calendar | Le calendrier à supprimer. |

### Valeur de retour

Si supprimé, renvoie true, sinon renvoie false.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancée lorsque le calendrier ne peut pas être supprimé. |

## Exemples

Montre comment remplacer un calendrier dans la collection.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// ajouter un nouveau calendrier
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


