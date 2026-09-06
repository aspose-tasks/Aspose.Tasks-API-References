---
title: "CsvOptions.Encoding"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CsvOptions. Obtient ou définit un encodage avec lequel enregistrer le CSV"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Obtient ou définit un encodage avec lequel enregistrer le CSV.

```csharp
public Encoding Encoding { get; set; }
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


