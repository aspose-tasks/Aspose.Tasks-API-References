---
title: "CsvOptions.TextDelimiter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CsvOptions. Ottiene o imposta un delimitatore di testo"
type: docs
weight: 50
url: /it/net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

Ottiene o imposta un delimitatore di testo.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
```

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

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


