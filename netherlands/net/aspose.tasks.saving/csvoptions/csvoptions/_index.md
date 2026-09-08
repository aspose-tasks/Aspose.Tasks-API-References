---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CsvOptions-constructor. Initialiseert een nieuw exemplaar van de CsvOptions-klasse die kan worden gebruikt om een project op te slaan in CSV-formaat"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Initialiseert een nieuw exemplaar van de [`CsvOptions`](../)-klasse die kan worden gebruikt om een project op te slaan in CSV-formaat.

```csharp
public CsvOptions()
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


