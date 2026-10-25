---
title: "Enum YearLabelDisplay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.YearLabelDisplay enum. Spécifie comment l’étiquette d’année s’affiche."
type: docs
weight: 3680
url: /fr/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Spécifie comment l'étiquette d'année s'affiche.

```csharp
public enum YearLabelDisplay
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Y | `0` | Définit la liste des années dans MS Project comme mo. |
| Yr | `1` | Définit la liste des années dans MS Project comme mon. |
| Year | `2` | Définit la liste des années dans MS Project comme mois. |

## Exemples

Montre comment définir l'étiquette d'année des options d'affichage du projet (cas 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// définir comment l'étiquette d'année est affichée
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


