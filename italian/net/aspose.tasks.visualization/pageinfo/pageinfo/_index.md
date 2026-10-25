---
title: "PageInfo.PageInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PageInfo costruttore. Inizializza una nuova istanza della classe PageInfo. Rappresenta i dati di configurazione della pagina presenti nel formato file MPP e utilizzati per la stampa"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/pageinfo/pageinfo/
---
## PageInfo constructor

Inizializza una nuova istanza della classe [`PageInfo`](../). Rappresenta i dati di configurazione della pagina presenti nel formato file MPP e utilizzati per la stampa.

```csharp
public PageInfo()
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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


