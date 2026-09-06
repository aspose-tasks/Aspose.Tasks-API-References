---
title: "Enum CostAccrualType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.CostAccrualType enum. Spécifie le type d'un coût d'accumulation"
type: docs
weight: 350
url: /fr/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Spécifie le type d’un coût d’accumulation.

```csharp
public enum CostAccrualType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que la valeur indéfinie signifie que le champ n'était pas défini dans le fichier de projet original. |
| Start | `0` | Indique le type d'accumulation de coût Start. |
| Prorated | `1` | Indique le type d'accumulation de coût Prorated. |
| End | `2` | Indique le type d'accumulation de coût End. |
| Invalid | `3` | Indique le type d'accumulation de coût Invalid. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment et quand les coûts standard et supplémentaires des ressources doivent être facturés ou accumulés (méthode d'accumulation : Détermine quand le coût d'une ressource est engagé et quand les coûts réels sont facturés à un projet. Vous pouvez engager les coûts au début [Start] ou à la fin [End] d'une tâche ou les proratiser [Prorated] pendant la tâche.), au coût d'une tâche (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// définir le type d'accumulation de coût
// si vous sélectionnez l'option End, les coûts ne sont pas accumulés tant que le travail restant n'est pas nul.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


