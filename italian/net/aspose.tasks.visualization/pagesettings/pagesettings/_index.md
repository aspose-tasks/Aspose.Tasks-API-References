---
title: "PageSettings.PageSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PageSettings. Inizializza una nuova istanza della classe PageSettings. Rappresenta le impostazioni di stampa per una pagina della visualizzazione del progetto."
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/pagesettings/pagesettings/
---
## PageSettings constructor

Inizializza una nuova istanza della classe [`PageSettings`](../). Rappresenta le impostazioni di stampa per una pagina della visualizzazione del progetto.

```csharp
public PageSettings()
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


