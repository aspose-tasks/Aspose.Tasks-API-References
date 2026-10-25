---
title: "PageInfo.Legend"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageInfo. Obtient ou définit une instance de la classe PageLegend qui spécifie les options de rendu de la légende de la page"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Obtient ou définit une instance de la classe [`PageLegend`](../../pagelegend/) qui spécifie les options de rendu de la légende de la page.

```csharp
public PageLegend Legend { get; set; }
```

## Remarques

Actuellement applicable uniquement aux vues de diagramme de Gantt.

## Exemples

Montre comment travailler avec les informations de légende de page.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// lisons les informations de légende de page
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// la modification d'une légende est également prise en charge
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


