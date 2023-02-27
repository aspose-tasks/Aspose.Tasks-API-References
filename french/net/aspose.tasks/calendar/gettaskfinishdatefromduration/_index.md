---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Calendar méthode. Calcule la date et lheure de fin de la tâche à partir de sa date de début des parties fractionnées et de la durée.
type: docs
weight: 190
url: /fr/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calcule la date et l'heure de fin de la tâche à partir de sa date de début, des parties fractionnées et de la durée.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| task | Task | La tâche pour laquelle obtenir la date de fin. |
| duration | TimeSpan | La durée de la tâche sur laquelle fractionner. |

### Return_Value

Date de fin de la tâche.

### Remarques

Renvoie DateTime.MinValue si la tâche est récapitulative, nulle ou si sa date de début n'est pas définie.

### Voir également

* class [Task](../../task/)
* class [Calendar](../)
* espace de noms [Aspose.Tasks](../../calendar/)
* Assemblée [Aspose.Tasks](../../../)


