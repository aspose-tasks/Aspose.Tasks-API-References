---
title: "Classe PageSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.PageSettings. Rappresenta le impostazioni di stampa per una pagina della visualizzazione del progetto"
type: docs
weight: 3240
url: /it/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Rappresenta le impostazioni di stampa per una pagina della visualizzazione del progetto.

```csharp
public class PageSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageSettings](pagesettings/)() | Inizializza una nuova istanza della classe `PageSettings`. Rappresenta le impostazioni di stampa per una pagina della visualizzazione del progetto. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Ottiene o imposta un valore che indica se regolare la stampa alla percentuale specificata ([`PercentOfNormalSize`](./percentofnormalsize/)) della dimensione normale. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Ottiene o imposta il numero della prima pagina per la stampa. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Ottiene o imposta il numero di pagine in altezza da stampare. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Ottiene o imposta il numero di pagine in larghezza da stampare. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Ottiene o imposta una dimensione della carta. Può essere uno dei valori dell'enumerazione [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Ottiene o imposta un intero che rappresenta uno dei valori di PrinterPaperSize o un ID di dimensione pagina personalizzata. Questo valore può essere usato per ottenere PaperSize dalle impostazioni del sistema operativo. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Ottiene o imposta una percentuale della dimensione normale a cui regolare la stampa. |

## Esempi

Mostra come lavorare con &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// ottieni le impostazioni
var settings = project.DefaultView.PageInfo.PageSettings;
// regoliamo alcune proprietà
// imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.
settings.IsPortrait = true;
// imposta il numero di pagine in larghezza da stampare.
settings.PagesInWidth = 5;
// imposta il numero di pagine in altezza da stampare.
settings.PagesInHeight = 7;
// imposta una percentuale della dimensione normale a cui regolare la stampa.
settings.PercentOfNormalSize = 200;
// imposta una dimensione della carta. Può essere uno dei valori dell'enumerazione <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// imposta il numero della prima pagina per la stampa.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


