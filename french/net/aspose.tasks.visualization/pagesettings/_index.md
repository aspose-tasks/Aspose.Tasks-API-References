---
title: "Classe PageSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageSettings. Représente les paramètres d'impression pour une page de la vue du projet"
type: docs
weight: 3240
url: /fr/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Représente les paramètres d'impression pour une page de la vue du projet.

```csharp
public class PageSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageSettings](pagesettings/)() | Initialise une nouvelle instance de la classe `PageSettings`. Représente les paramètres d'impression pour une page de la vue du projet. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié ([`PercentOfNormalSize`](./percentofnormalsize/)) de la taille normale. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Obtient ou définit le numéro de première page pour l'impression. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Obtient ou définit le nombre de pages en hauteur à imprimer. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Obtient ou définit le nombre de pages en largeur à imprimer. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Obtient ou définit une taille de papier. Peut être l'une des valeurs de l'énumération [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Obtient ou définit un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. Cette valeur peut être utilisée pour obtenir PaperSize à partir des paramètres du système d'exploitation. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Obtient ou définit un pourcentage de la taille normale auquel ajuster l'impression. |

## Exemples

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// obtenir les paramètres
var settings = project.DefaultView.PageInfo.PageSettings;
// ajustons quelques propriétés
// définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.
settings.IsPortrait = true;
// définit le nombre de pages en largeur à imprimer.
settings.PagesInWidth = 5;
// définit le nombre de pages en hauteur à imprimer.
settings.PagesInHeight = 7;
// définit un pourcentage de la taille normale auquel ajuster l'impression.
settings.PercentOfNormalSize = 200;
// définit une taille de papier. Peut être l'une des valeurs de l'énumération <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// définit le numéro de première page pour l'impression.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


