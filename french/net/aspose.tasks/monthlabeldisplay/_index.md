---
title: "Enum MonthLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.MonthLabelDisplay enum. Spécifie comment l'étiquette du mois s'affiche"
type: docs
weight: 1060
url: /fr/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Spécifie comment l'étiquette du mois s'affiche.

```csharp
public enum MonthLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Mo | `0` | Définit la liste des mois dans MS Project comme mo. |
| Mon | `1` | Définit la liste des mois dans MS Project comme mon. |
| Month | `2` | Définit la liste des mois dans MS Project comme month. |

## Exemples

Montre comment définir l'étiquette du mois des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définir comment l'étiquette du mois est affichée
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


