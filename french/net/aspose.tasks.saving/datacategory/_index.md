---
title: "Enum DataCategory"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.Saving.DataCategory. La catégorie de données utilisée lors de l'enregistrement au format CSV"
type: docs
weight: 2000
url: /fr/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

La catégorie de données utilisée lors de l'enregistrement au format CSV.

```csharp
public enum DataCategory
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Tasks | `0` | Informations sur les tâches. |
| Resources | `1` | Informations sur les ressources. |
| Assignments | `2` | Informations sur les affectations. |

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


