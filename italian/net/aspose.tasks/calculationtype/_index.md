---
title: "Enum CalculationType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CalculationType enum. Specifica il tipo di calcolo del valore degli attributi personalizzati"
type: docs
weight: 220
url: /it/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Specifica il tipo di calcolo del valore dell'attributo personalizzato.

```csharp
public enum CalculationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Indica che l'attributo esteso non ha una tabella di ricerca o formula e memorizza semplicemente il valore impostato dall'utente. |
| Lookup | `1` | Indica che il valore dell'attributo esteso è limitato ai valori provenienti da una tabella di ricerca. |
| Formula | `2` | Indica che il valore dell'attributo esteso è calcolato utilizzando la formula definita in [`Formula`](../extendedattributedefinition/formula/). |

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


