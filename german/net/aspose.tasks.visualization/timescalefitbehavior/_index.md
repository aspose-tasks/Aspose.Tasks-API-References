---
title: "Enum TimescaleFitBehavior"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior enum. Stellt ein Verhalten dar, das verwendet wird, um den Zeitskalenbereich an die Seitenbreite anzupassen"
type: docs
weight: 3440
url: /de/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Stellt ein Verhalten dar, das verwendet wird, um den Zeitskalenbereich an die Seitenbreite anzupassen.

```csharp
public enum TimescaleFitBehavior
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DefinedInView | `0` | Kalenderabschnitt wird gemäß der Eigenschaft View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage der gerenderten Ansicht dargestellt. |
| NoScaleToEndDate | `1` | Kalenderabschnitt wird exakt bis zum Enddatum dargestellt, selbst wenn auf einer Seite ein leerer Raum vorhanden ist. |
| NoScaleToEndOfPage | `2` | Kalenderabschnitt wird bis zum Ende (rechte Seite) der letzten Seite dargestellt. Daher kann das zuletzt gerenderte Datum das Enddatum überschreiten. |
| ScaleToEndOfPage | `3` | Die Rendering-Engine versucht, die Daten so auszurichten, dass das Enddatum mit dem Ende (rechte Seite) der letzten Seite übereinstimmt. Entspricht der aktivierten Option "Page Setup \ View \ Fit timescale to end of page" von MS Project. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


