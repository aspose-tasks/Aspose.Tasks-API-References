---
title: "Enum HourLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.HourLabelDisplay. Spécifie comment l'étiquette d'heure s'affiche"
type: docs
weight: 820
url: /fr/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Spécifie comment l'étiquette de l'heure s'affiche.

```csharp
public enum HourLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| H | `0` | "h" étiquette. |
| Hr | `1` | "hr" étiquette. |
| Hour | `2` | "hour(s)" étiquette. |

## Exemples

Montre comment définir l'étiquette d'heure des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définir comment l'étiquette d'heure est affichée
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


