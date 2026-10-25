---
title: "Project.GetBaselineSaveTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Restituisce il tempo di salvataggio della baseline"
type: docs
weight: 1090
url: /it/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Restituisce il tempo di salvataggio della baseline.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baselineNumber | BaselineType | Il numero della baseline [`BaselineType`](../../baselinetype/). |

### Valore di ritorno

La data e l'ora dell'ultimo salvataggio della baseline.

## Osservazioni

Restituisce DateTime.MinValue se la baseline non è stata salvata.

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


