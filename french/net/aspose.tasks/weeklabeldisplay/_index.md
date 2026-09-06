---
title: "Enum WeekLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.WeekLabelDisplay enum. Spécifie comment l'étiquette de semaine s'affiche"
type: docs
weight: 3560
url: /fr/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Spécifie comment l'étiquette de semaine s'affiche.

```csharp
public enum WeekLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| W | `0` | "w" étiquette. |
| Wk | `1` | "wk" étiquette. |
| Week | `2` | "week" étiquette. |

## Exemples

Montre comment définir l'étiquette de semaine des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définir comment l'étiquette de la semaine s'affiche
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


