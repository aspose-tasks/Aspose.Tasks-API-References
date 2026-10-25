---
title: "Enum CsvTextDelimiter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.CsvTextDelimiter enum. Tekstscheidingsteken voor CSV-formaat"
type: docs
weight: 1990
url: /nl/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Tekstscheidingsteken voor CSV-indeling.

```csharp
public enum CsvTextDelimiter
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Comma | `0` | Komma‑scheidingsteken. |
| Semicolon | `1` | Puntkomma‑scheidingsteken. |
| Space | `2` | Spatie‑scheidingsteken. |
| Tab | `3` | Tab‑scheidingsteken. |

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


