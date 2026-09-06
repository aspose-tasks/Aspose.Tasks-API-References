---
title: "Énumération CsvTextDelimiter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Saving.CsvTextDelimiter. Délimiteur de texte pour le format CSV"
type: docs
weight: 1990
url: /fr/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Délimiteur de texte pour le format CSV.

```csharp
public enum CsvTextDelimiter
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Comma | `0` | Délimiteur virgule. |
| Semicolon | `1` | Délimiteur point-virgule. |
| Space | `2` | Délimiteur espace. |
| Tab | `3` | Délimiteur tabulation. |

## Exemples

Montre comment utiliser &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; pour enregistrer un projet au format CSV.

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

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


