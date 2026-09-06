---
title: "PageViewSettings.PrintAllSheetColumns"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageViewSettings. Obtient ou définit une valeur indiquant s'il faut imprimer toutes les colonnes de feuille d'une vue"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/
---
## PageViewSettings.PrintAllSheetColumns property

Obtient ou définit une valeur indiquant s'il faut imprimer toutes les colonnes de la feuille d'une vue.

```csharp
public bool PrintAllSheetColumns { get; set; }
```

## Exemples

Montre comment imprimer les notes de tâche, de ressource et d'affectation sur une page séparée.

```csharp
var project = new Project(DataDir + "Input.mpp");

// définissez le nombre de premières colonnes à imprimer sur toutes les pages
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// définir une valeur indiquant s'il faut imprimer les notes.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// définir une valeur indiquant s'il faut ajuster l'échelle de temps à la fin d'une page lors de l'impression.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// définir une valeur indiquant s'il faut imprimer toutes les colonnes de la feuille d'une vue
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// définir une valeur indiquant s'il faut imprimer les pages vierges d'une vue
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// définissez une valeur indiquant s'il faut imprimer un nombre spécifié de premières colonnes sur toutes les pages
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


