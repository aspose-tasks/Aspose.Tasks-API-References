---
title: "Classe PageViewSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageViewSettings. Représente les paramètres d'impression pour une vue de projet"
type: docs
weight: 3260
url: /fr/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Représente les paramètres d'impression pour une vue du projet.

```csharp
public class PageViewSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Obtient ou définit le nombre de premières colonnes à imprimer sur toutes les pages. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut ajuster l'échelle de temps à la fin d'une page lors de l'impression. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut imprimer toutes les colonnes de la feuille d'une vue. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut imprimer les pages vierges d'une vue. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut imprimer un nombre spécifié de premières colonnes sur toutes les pages. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut imprimer les notes. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


