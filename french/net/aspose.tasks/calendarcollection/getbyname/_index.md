---
title: "CalendarCollection.GetByName"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Retourne un calendrier avec le nom spécifié."
type: docs
weight: 30
url: /fr/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Renvoie un calendrier avec le nom spécifié.

```csharp
public Calendar GetByName(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | Chaîne | Nom d'un calendrier. |

### Valeur de retour

Si trouvé, retourne le calendrier avec le nom spécifié sinon retourne null.

## Exemples

Montre comment obtenir des calendriers par nom ou par identifiant.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


