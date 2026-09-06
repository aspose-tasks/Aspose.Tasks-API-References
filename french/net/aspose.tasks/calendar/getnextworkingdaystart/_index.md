---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Calcule le début du prochain jour ouvrable pour la date spécifiée"
type: docs
weight: 180
url: /fr/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Calcule le début du prochain jour ouvrable pour la date spécifiée.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| date | DateTime | La date pour laquelle obtenir le début du prochain jour ouvrable. |

### Valeur de retour

DateTime du début du prochain jour ouvrable.

## Exemples

Montre comment obtenir le début du prochain jour ouvrable en utilisant un calendrier.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenir le début du prochain jour ouvrable (le week-end est ignoré)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// Le 13 avril 2020 09:00 sera imprimé
Console.WriteLine(nextWorkingDayStart);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


