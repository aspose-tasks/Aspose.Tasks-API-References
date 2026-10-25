---
title: "Classe PageInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.PageInfo. Rappresenta i dati di configurazione della pagina presenti nel formato file MPP e utilizzati per la stampa."
type: docs
weight: 3200
url: /it/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Rappresenta i dati di impostazione della pagina presenti nel formato file MPP e utilizzati per la stampa.

```csharp
public class PageInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageInfo](pageinfo/)() | Inizializza una nuova istanza della classe `PageInfo`. Rappresenta i dati di configurazione della pagina presenti nel formato file MPP e utilizzati per la stampa. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Ottiene o imposta un'istanza della classe [`HeaderFooterInfo`](../headerfooterinfo/) che rappresenta i dati del piè di pagina. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Ottiene o imposta l'istanza della classe [`HeaderFooterInfo`](../headerfooterinfo/) che rappresenta i dati dell'intestazione. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Ottiene o imposta un'istanza della classe [`PageLegend`](../pagelegend/) che specifica le opzioni di rendering della legenda della pagina. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Ottiene un'istanza della classe [`PageMargins`](../pagemargins/) che specifica i margini della pagina. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Ottiene il nome della vista per la quale vengono utilizzati i dati di configurazione. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Ottiene un'istanza della classe [`PageSettings`](./pagesettings/) che specifica le impostazioni di stampa della pagina. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Ottiene un'istanza della classe [`PageViewSettings`](./pageviewsettings/) che specifica le impostazioni di stampa della vista della pagina. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


