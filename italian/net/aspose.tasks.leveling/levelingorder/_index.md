---
title: "Enum LevelingOrder"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Leveling.LevelingOrder. Definisce i possibili valori dell'ordine di livellamento"
type: docs
weight: 950
url: /it/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Definisce i possibili valori dell'ordine di livellamento.

```csharp
public enum LevelingOrder
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Standard | `1` | Le seguenti proprietà sono prese in considerazione: relazioni di predecessore, margine totale (un'attività con margine totale più alto è ritardata per prima), data di inizio, priorità. Questo è il valore predefinito. |
| IdOnly | `2` | Le attività sono ritardate in ordine crescente di Id. |
| PriorityThenStandard | `3` | La priorità è considerata per prima, poi le stesse proprietà di Standard. |

### Vedi anche

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


