---
title: "Énumération CalculationType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.CalculationType enum. Spécifie le type de calcul de la valeur des attributs personnalisés"
type: docs
weight: 220
url: /fr/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Spécifie le type de calcul de la valeur de l’attribut personnalisé.

```csharp
public enum CalculationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Signifie que l'attribut étendu n'a pas de table de recherche de formule et stocke simplement la valeur définie par l'utilisateur. |
| Lookup | `1` | Signifie que la valeur de l'attribut étendu est limitée aux valeurs d'une table de recherche. |
| Formula | `2` | Signifie que la valeur de l'attribut étendu est calculée à l'aide de la formule définie dans [`Formula`](../extendedattributedefinition/formula/). |

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


