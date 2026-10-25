---
title: "CsvOptions.CsvOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore CsvOptions. Inizializza una nuova istanza della classe CsvOptions che può essere utilizzata per salvare il progetto in formato CSV"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Inizializza una nuova istanza della classe [`CsvOptions`](../) che può essere utilizzata per salvare il progetto in formato CSV.

```csharp
public CsvOptions()
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


