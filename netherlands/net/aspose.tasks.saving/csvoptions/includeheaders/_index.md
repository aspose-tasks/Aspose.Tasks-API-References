---
title: "CsvOptions.IncludeHeaders"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CsvOptions property. Haalt op of stelt een waarde in die aangeeft of kopteksten moeten worden opgenomen of niet; standaardwaarde is TRUE"
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Haalt op of stelt een waarde in die aangeeft of kopteksten al dan niet moeten worden opgenomen (standaardwaarde is TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


