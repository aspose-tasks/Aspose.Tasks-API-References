---
title: "Enum DataCategory"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.DataCategory‑enum. De categorie gegevens die wordt gebruikt bij het opslaan naar CSV."
type: docs
weight: 2000
url: /nl/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

De categorie van gegevens die wordt gebruikt bij het opslaan naar CSV.

```csharp
public enum DataCategory
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Tasks | `0` | Taakinformatie. |
| Resources | `1` | Resource‑informatie. |
| Assignments | `2` | Toewijzingsinformatie. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


