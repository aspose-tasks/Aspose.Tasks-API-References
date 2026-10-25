---
title: "PageInfo.Legend"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PageInfo proprietà. Ottiene o imposta un'istanza della classe PageLegend che specifica le opzioni di rendering della legenda della pagina"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Ottiene o imposta un'istanza della classe [`PageLegend`](../../pagelegend/) che specifica le opzioni di rendering della legenda della pagina.

```csharp
public PageLegend Legend { get; set; }
```

## Osservazioni

Attualmente è applicabile solo alle visualizzazioni Gantt Chart.

## Esempi

Mostra come lavorare con le informazioni della legenda della pagina.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// consente di leggere le informazioni della legenda della pagina
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// anche la modifica di una legenda è supportata
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

Mostra come lavorare con le informazioni della pagina nella vista di MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// consente di modificare la vista predefinita
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// consente di modificare i margini
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// consente di modificare le impostazioni della pagina
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// consente di modificare le impostazioni della vista della pagina
// imposta un valore che indica se stampare le note.
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

// lavorare con il progetto...
```

### Vedi anche

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


