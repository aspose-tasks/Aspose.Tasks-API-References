---
title: "CsvOptions.CsvOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur CsvOptions. Initialise une nouvelle instance de la classe CsvOptions qui peut être utilisée pour enregistrer le projet au format CSV"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Initialise une nouvelle instance de la classe [`CsvOptions`](../) qui peut être utilisée pour enregistrer le projet au format CSV.

```csharp
public CsvOptions()
```

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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


