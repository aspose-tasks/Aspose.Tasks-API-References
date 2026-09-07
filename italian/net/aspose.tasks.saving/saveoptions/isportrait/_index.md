---
title: "SaveOptions.IsPortrait"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale."
type: docs
weight: 70
url: /it/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

```csharp
public bool IsPortrait { get; set; }
```

## Osservazioni

Non è applicabile quando SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In questo caso viene utilizzato View.PageInfo.PageSettings.IsPortrait. Non è applicabile quando SaveOptions.CustomPageSize è impostato.

## Esempi

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


