---
title: "Calendar.GetWorkingTimes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Retourne WorkingTimeCollection des heures de travail pour la date spécifiée"
type: docs
weight: 240
url: /fr/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Retourne [`WorkingTimeCollection`](../../workingtimecollection/) des créneaux de travail pour la date spécifiée.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dt | DateTime | La date pour laquelle obtenir les heures de travail. |

### Valeur de retour

Collection d'instances de [`WorkingTime`](../../workingtime/).

## Exemples

Montre comment obtenir les heures de travail pour une date spécifique.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenir les heures de travail pour une date spécifique
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 heures seront affichées
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Voir aussi

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


