---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttributeDefinition. Ottiene o imposta il tipo di calcolo del valore degli attributi personalizzati per le righe di riepilogo"
type: docs
weight: 260
url: /it/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

## Esempi

Mostra come lavorare con il tipo di calcolo di una definizione di attributo esteso.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crea una definizione di attributo con tipo 'Formula' dove i valori per le attività foglia e le attività riepilogo sono calcolati usando la formula.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// crea una definizione di attributo dove i valori per le attività riepilogo sono calcolati usando il tipo di aggregazione 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Vedi anche

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


