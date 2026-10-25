---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Calcule la fin de la journée de travail précédente à partir de la date spécifiée"
type: docs
weight: 190
url: /fr/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Calcule la fin du jour ouvrable précédent à partir de la date spécifiée.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| date | DateTime | la date pour calculer la fin du jour ouvrable précédent. |

### Valeur de retour

La fin de la fin du jour ouvrable précédent.

## Exemples

Montre comment obtenir la fin de la journée de travail précédente en utilisant un calendrier.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenir la fin de la journée de travail précédente
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// Le 9 avril 2020 18:00 PM sera imprimé.
Console.WriteLine(previousWorkingDayEnd);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


