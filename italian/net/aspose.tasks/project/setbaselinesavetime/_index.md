---
title: "Project.SetBaselineSaveTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Project. Imposta il tempo di salvataggio della baseline"
type: docs
weight: 1260
url: /it/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Imposta l'ora di salvataggio della baseline.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baselineNumber | BaselineType | Il numero della baseline [`BaselineType`](../../baselinetype/). |
| valore | DateTime | La data e l'ora dell'ultimo salvataggio della baseline. |

## Osservazioni

Imposta il valore a DateTime.MinValue se la baseline non è stata salvata.

## Esempi

Mostra come leggere/scrivere il tempo di salvataggio della baseline del progetto.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// imposta tempo di salvataggio della baseline
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Vedi anche

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


