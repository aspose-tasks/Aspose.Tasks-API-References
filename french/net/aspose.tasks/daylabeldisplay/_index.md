---
title: "Enum DayLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.DayLabelDisplay enum. Spécifie comment l'étiquette de jour s'affiche"
type: docs
weight: 440
url: /fr/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Spécifie comment l'étiquette du jour s'affiche.

```csharp
public enum DayLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| D | `0` | Définit la liste des jours dans MS Project comme d. |
| Dy | `1` | Définit la liste des jours dans MS Project comme dy. |
| Day | `2` | Définit la liste des jours dans MS Project comme day. |

## Exemples

Montre comment définir l'étiquette de jour des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définir comment l'étiquette du jour s'affiche
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


