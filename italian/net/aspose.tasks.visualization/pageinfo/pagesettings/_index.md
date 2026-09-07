---
title: "PageInfo.PageSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PageInfo proprietà. Ottiene un'istanza della classe PageSettings che specifica le impostazioni di stampa della pagina"
type: docs
weight: 70
url: /it/net/aspose.tasks.visualization/pageinfo/pagesettings/
---
## PageInfo.PageSettings property

Ottiene un'istanza della classe `PageSettings` che specifica le impostazioni di stampa della pagina.

```csharp
public PageSettings PageSettings { get; }
```

## Esempi

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

* class [PageSettings](../../pagesettings/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


