---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SaveOptions‑Eigenschaft. Lässt ein Verhalten zu, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird."
type: docs
weight: 210
url: /de/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Liest oder setzt ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Beispiele

Zeigt, wie man TimescaleFitBehavior verwendet, um die Zeitskala des Gantt-Diagramms bis zum Ende der letzten Seite anzupassen.

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

### Siehe auch

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


