---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SaveOptions‑Eigenschaft. Lässt einen Wert zu, der definiert, wie eine Legende gerendert wird. Der Standardwert ist LegendDrawingOptions.OnEveryPage."
type: docs
weight: 80
url: /de/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Liest oder setzt einen Wert, der definiert, wie eine Legende gerendert wird. Der Standardwert ist LegendDrawingOptions.OnEveryPage.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Hinweise

Gilt nur, wenn die Gantt‑Diagrammansicht gerendert wird.

## Beispiele

Zeigt, wie die Legende auf der letzten Seite gedruckt wird.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Legendenzeichnungsoptionen aus der Ansicht übernehmen.
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Zeigt, wie Seitenlegenden ausgeblendet werden.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Geben Sie LegendDrawingOptions.NoLegend an, um Legenden auszublenden.
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

Zeigt, wie die Option LegendDrawingOptions.DefinedInView verwendet wird.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Legendenzeichnungsoptionen aus der Ansicht übernehmen.
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

Zeigt, wie Aufgabenbalken in der Seitenlegende des Gantt-Diagramms angepasst werden können.

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

### Siehe auch

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


