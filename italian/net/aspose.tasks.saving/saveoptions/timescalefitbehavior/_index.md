---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina"
type: docs
weight: 210
url: /it/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Esempi

Mostra come utilizzare TimescaleFitBehavior per far adattare la scala temporale del Gantt chart alla fine dell'ultima pagina.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Vedi anche

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


