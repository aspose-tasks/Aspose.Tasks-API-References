---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttributeDefinition. Obtient ou définit le type de calcul de la valeur des attributs personnalisés pour les lignes de résumé"
type: docs
weight: 260
url: /fr/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


