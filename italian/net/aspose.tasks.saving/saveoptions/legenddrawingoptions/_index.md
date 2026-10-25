---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che definisce come rendere una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage"
type: docs
weight: 80
url: /it/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Ottiene o imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Osservazioni

È applicabile solo quando la vista del diagramma di Gantt viene renderizzata.

## Esempi

Mostra come stampare la legenda nell'ultima pagina

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Prendi le opzioni di disegno della legenda dalla vista
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Mostra come nascondere le legende delle pagine.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Specifica LegendDrawingOptions.NoLegend per nascondere le legende
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

Mostra come usare l'opzione LegendDrawingOptions.DefinedInView.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Prendi le opzioni di disegno della legenda dalla vista
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

Mostra come personalizzare le barre delle attività nella legenda di pagina del diagramma di Gantt.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### Vedi anche

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


