---
title: "Enum RollupType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.RollupType enum. Spécifie le type de regroupement"
type: docs
weight: 1950
url: /fr/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Spécifie le type d'agrégation.

```csharp
public enum RollupType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Null | `0` | Indique le type de regroupement Null. |
| Maximum | `1` | Indique le type de regroupement Maximum. |
| Minimum | `2` | Indique le type de regroupement Minimum. |
| Count | `3` | Indique le type de regroupement Count. |
| Sum | `4` | Indique le type de regroupement Sum. |
| Average | `5` | Indique le type de regroupement Average. |
| AverageFirstSublevel | `6` | Indique le type de regroupement Average First Sublevel. |
| CountFirstSublevel | `7` | Indique le type de regroupement Count First Sublevel. |
| CountNonsummaries | `8` | Indique le type de regroupement Count Non-Summaries. |

## Exemples

Montre comment travailler avec le type de calcul d'une définition d'attribut étendu.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// créer une définition d'attribut avec le type 'Formula' où les valeurs des tâches feuilles et des tâches récapitulatives sont calculées à l'aide d'une formule.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// créer une définition d'attribut où les valeurs des tâches récapitulatives sont calculées à l'aide du type de regroupement 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


