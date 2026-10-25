---
title: "CsvOptions.IncludeHeaders"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CsvOptions. Obtient ou définit une valeur indiquant s'il faut inclure les en-têtes ou non ; la valeur par défaut est TRUE"
type: docs
weight: 40
url: /fr/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Obtient ou définit une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


