---
title: "CsvOptions.DataCategory"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CsvOptions. Ottiene o imposta una categoria di dati da salvare"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Ottiene o imposta una categoria di dati da salvare.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


