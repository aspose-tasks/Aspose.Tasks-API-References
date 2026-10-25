---
title: "PageInfo.PageViewSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageInfo. Obtient une instance de la classe PageViewSettings qui spécifie les paramètres d’impression de la vue de page"
type: docs
weight: 80
url: /fr/net/aspose.tasks.visualization/pageinfo/pageviewsettings/
---
## PageInfo.PageViewSettings property

Obtient une instance de la classe `PageViewSettings` qui spécifie les paramètres d’impression de la vue de page.

```csharp
public PageViewSettings PageViewSettings { get; }
```

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

* class [PageViewSettings](../../pageviewsettings/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


