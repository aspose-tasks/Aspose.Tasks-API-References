---
title: "Enum TimescaleFitBehavior"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Visualization.TimescaleFitBehavior. Rappresenta un comportamento usato per allineare l'area della scala temporale alla larghezza della pagina."
type: docs
weight: 3440
url: /it/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Rappresenta un comportamento utilizzato per allineare l'area della scala temporale alla larghezza della pagina.

```csharp
public enum TimescaleFitBehavior
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DefinedInView | `0` | La sezione del calendario è renderizzata secondo la proprietà View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage della vista renderizzata. |
| NoScaleToEndDate | `1` | La sezione del calendario è renderizzata esattamente fino a EndDate, anche se c'è uno spazio vuoto su una pagina. |
| NoScaleToEndOfPage | `2` | La sezione del calendario è renderizzata fino alla fine (lato destro) dell'ultima pagina. Pertanto la data renderizzata più recente può superare EndDate. |
| ScaleToEndOfPage | `3` | Il motore di rendering cercherà di allineare le date in modo che EndDate sia allineato con la fine (lato destro) dell'ultima pagina. Corrisponde all'opzione \"Impostazione pagina \\ Vista \\ Adatta scala temporale alla fine della pagina\" di MS Project abilitata. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


