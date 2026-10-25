---
title: "CalendarCollection.GetByUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode CalendarCollection. Retourne un calendrier avec l'UID spécifié"
type: docs
weight: 40
url: /fr/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Renvoie un calendrier avec l'UID spécifié.

```csharp
public Calendar GetByUid(int uid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID d'un calendrier. |

### Valeur de retour

Calendrier avec un UID spécifié.

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


