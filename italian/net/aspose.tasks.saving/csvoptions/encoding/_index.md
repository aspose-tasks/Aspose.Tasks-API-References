---
title: "CsvOptions.Encoding"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CsvOptions. Ottiene o imposta una codifica con cui salvare il CSV"
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Ottiene o imposta una codifica con cui salvare il CSV.

```csharp
public Encoding Encoding { get; set; }
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


