---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ICalendar. Calcule la date et l'heure de fin de la tâche à partir de ses parties de date de début et de la durée de travail."
type: docs
weight: 50
url: /fr/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée du travail.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | La tâche pour laquelle calculer la date de fin. |
| duration | TimeSpan | La durée à calculer. |

### Valeur de retour

Date de fin de la tâche pour la date de début et la durée données.

## Remarques

Renvoie DateTime.MinValue si la tâche est un résumé, nulle ou si sa date de début n'est pas définie.

### Voir aussi

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


