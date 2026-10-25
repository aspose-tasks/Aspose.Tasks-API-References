---
title: "Classe PageInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageInfo. Représente les données de configuration de page présentes dans le format de fichier MPP et utilisées pour l'impression."
type: docs
weight: 3200
url: /fr/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Représente les données de configuration de page présentes dans le format de fichier MPP et utilisées pour l'impression.

```csharp
public class PageInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageInfo](pageinfo/)() | Initialise une nouvelle instance de la classe `PageInfo`. Représente les données de configuration de page présentes dans le format de fichier MPP et utilisées pour l'impression. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Obtient ou définit une instance de la classe [`HeaderFooterInfo`](../headerfooterinfo/) qui représente des données de pied de page. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Obtient ou définit l'instance de la classe [`HeaderFooterInfo`](../headerfooterinfo/) qui représente des données d'en-tête. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Obtient ou définit une instance de la classe [`PageLegend`](../pagelegend/) qui spécifie les options de rendu de la légende de page. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Obtient une instance de la classe [`PageMargins`](../pagemargins/) qui spécifie les marges de la page. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Obtient le nom de la vue pour laquelle les données de configuration sont utilisées. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Obtient une instance de la classe [`PageSettings`](./pagesettings/) qui spécifie les paramètres d'impression de la page. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Obtient une instance de la classe [`PageViewSettings`](./pageviewsettings/) qui spécifie les paramètres d'impression de la vue de page. |

## Exemples

Montre comment travailler avec les informations de page de la vue MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// modifions la vue par défaut
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// modifions les marges
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// modifions les paramètres de page
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// modifions les paramètres de vue de page
// définir une valeur indiquant s'il faut imprimer les notes.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


