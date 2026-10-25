---
title: "CsvOptions.Encoding"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CsvOptions-eigenschap. Haalt op of stelt een codering in om CSV mee op te slaan"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Haalt op of stelt een codering in waarmee CSV moet worden opgeslagen.

```csharp
public Encoding Encoding { get; set; }
```

## Voorbeelden

Toont hoe &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; te gebruiken om een project op te slaan als CSV-bestand.

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

### Zie ook

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


