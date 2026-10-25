---
title: "Enum RollupType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.RollupType enum. Specifica il tipo di aggregazione"
type: docs
weight: 1950
url: /it/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Specifica il tipo di aggregazione.

```csharp
public enum RollupType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Null | `0` | Indica il tipo di aggregazione Null. |
| Maximum | `1` | Indica il tipo di aggregazione Massimo. |
| Minimum | `2` | Indica il tipo di aggregazione Minimo. |
| Count | `3` | Indica il tipo di aggregazione Conteggio. |
| Sum | `4` | Indica il tipo di aggregazione Somma. |
| Average | `5` | Indica il tipo di aggregazione Media. |
| AverageFirstSublevel | `6` | Indica il tipo di aggregazione Media Primo SottoLivello. |
| CountFirstSublevel | `7` | Indica il tipo di aggregazione Conteggio Primo SottoLivello. |
| CountNonsummaries | `8` | Indica il tipo di aggregazione Conteggio Non-Riepiloghi. |

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


