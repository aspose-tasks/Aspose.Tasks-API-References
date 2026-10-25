---
title: "Énumération BaselineType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.BaselineType. Spécifie le type de ligne de base utilisé pour calculer les valeurs de variance."
type: docs
weight: 130
url: /fr/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Spécifie le type de ligne de base utilisé pour calculer les valeurs de variance.

```csharp
public enum BaselineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que le champ n'était pas défini dans le fichier de projet original. |
| Baseline | `0` | Indique le type de ligne de base. |
| Baseline1 | `1` | Indique le type de Baseline1. |
| Baseline2 | `2` | Indique le type de Baseline2. |
| Baseline3 | `3` | Indique le type de Baseline3. |
| Baseline4 | `4` | Indique le type de Baseline4. |
| Baseline5 | `5` | Indique le type de Baseline5. |
| Baseline6 | `6` | Indique le type de Baseline6. |
| Baseline7 | `7` | Indique le type de Baseline7. |
| Baseline8 | `8` | Indique le type de Baseline8. |
| Baseline9 | `9` | Indique le type de Baseline9. |
| Baseline10 | `10` | Indique le type de Baseline10. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment définir la ligne de base pour le projet (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Enregistre les champs de ligne de base dans la ligne de base spécifiée pour l'ensemble du projet.
project.SetBaseline(BaselineType.Baseline);
// Travailler avec les lignes de base du projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


