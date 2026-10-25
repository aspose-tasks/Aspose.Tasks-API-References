---
title: "CsvOptions.IncludeHeaders"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CsvOptions. Ottiene o imposta un valore che indica se includere le intestazioni o meno; il valore predefinito è TRUE"
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Ottiene o imposta un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


