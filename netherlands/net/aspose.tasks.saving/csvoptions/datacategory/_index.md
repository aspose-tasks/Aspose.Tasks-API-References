---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CsvOptions property. Haalt op of stelt een gegevenscategorie in die moet worden opgeslagen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Haalt op of stelt een gegevenscategorie in die moet worden opgeslagen.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


