---
title: "Enum SummaryRowsCalculationType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.SummaryRowsCalculationType. Specifica il tipo di calcolo del valore degli attributi personalizzati per le righe di riepilogo."
type: docs
weight: 2310
url: /it/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Specifica il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo.

```csharp
public enum SummaryRowsCalculationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Indica che il valore dell'attributo personalizzato per le righe di riepilogo non è calcolato. |
| Rollup | `1` | Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato usando la funzione di aggregazione definita in [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | Indica che il valore dell'attributo personalizzato per le righe di riepilogo è calcolato usando la formula definita in [`Formula`](../extendedattributedefinition/formula/). |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


