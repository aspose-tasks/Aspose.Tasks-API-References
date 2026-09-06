---
title: "CsvOptions.DataCategory"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CsvOptions. Obtient ou définit une catégorie de données à enregistrer"
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Obtient ou définit une catégorie de données à enregistrer.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


