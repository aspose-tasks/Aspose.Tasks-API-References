---
title: "PageSettings.PaperSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta una dimensione della carta. Può essere uno dei valori dell'enumerazione PrinterPaperSize"
type: docs
weight: 70
url: /it/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

Ottiene o imposta una dimensione della carta. Può essere uno dei valori dell'enumerazione [`PrinterPaperSize`](../../printerpapersize/).

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

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

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


