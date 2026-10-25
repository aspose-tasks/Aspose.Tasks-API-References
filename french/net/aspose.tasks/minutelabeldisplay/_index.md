---
title: "Énumération MinuteLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.MinuteLabelDisplay. Spécifie comment le libellé des minutes s'affiche"
type: docs
weight: 1030
url: /fr/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Spécifie comment l'étiquette des minutes s'affiche.

```csharp
public enum MinuteLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| M | `0` | Définit la liste des minutes dans MS Project comme m. |
| Min | `1` | Définit la liste des minutes dans MS Project comme min. |
| Minute | `2` | Définit la liste des minutes dans MS Project comme minute. |

## Exemples

Montre comment définir le libellé des minutes des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définit comment le libellé des minutes est affiché
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


