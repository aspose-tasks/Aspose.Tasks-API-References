---
title: "Enum DataCategory"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.DataCategory. La categoria di dati utilizzata durante il salvataggio in CSV"
type: docs
weight: 2000
url: /it/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

La categoria dei dati utilizzata durante il salvataggio in CSV.

```csharp
public enum DataCategory
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Tasks | `0` | Informazioni sulle attività. |
| Resources | `1` | Informazioni sulle risorse. |
| Assignments | `2` | Informazioni sulle assegnazioni. |

## Esempi

Mostra come utilizzare &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; per salvare un progetto come file CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


