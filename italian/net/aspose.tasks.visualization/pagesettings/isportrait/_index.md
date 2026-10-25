---
title: "PageSettings.IsPortrait"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale."
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

```csharp
public bool IsPortrait { get; set; }
```

## Osservazioni

È applicabile durante il rendering quando SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

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

Mostra come specificare la dimensione e l'orientamento della pagina utilizzando le impostazioni di View o utilizzando SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// In questo caso la dimensione e l'orientamento della pagina vengono applicati dalle proprietà view.PageInfo.PageSettings.PaperSize e view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// In questo caso la dimensione e l'orientamento della pagina vengono applicati dalle proprietà di SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// In questo caso la dimensione della pagina viene applicata da SaveOptions.CustomPageSize. La proprietà IsPortrait non viene considerata.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Vedi anche

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


