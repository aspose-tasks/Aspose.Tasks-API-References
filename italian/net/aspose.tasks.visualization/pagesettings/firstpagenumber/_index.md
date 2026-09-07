---
title: "PageSettings.FirstPageNumber"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta il numero della prima pagina per la stampa"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

Ottiene o imposta il numero della prima pagina per la stampa.

```csharp
public short FirstPageNumber { get; set; }
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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


