---
title: "Enum CsvTextDelimiter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.CsvTextDelimiter. Delimitatore di testo per il formato CSV"
type: docs
weight: 1990
url: /it/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Delimitatore di testo per il formato CSV.

```csharp
public enum CsvTextDelimiter
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Comma | `0` | Delimitatore di virgola. |
| Semicolon | `1` | Delimitatore di punto e virgola. |
| Space | `2` | Delimitatore di spazio. |
| Tab | `3` | Delimitatore di tabulazione. |

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


