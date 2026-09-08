---
title: "Перечисление TimescaleFitBehavior"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.TimescaleFitBehavior. Представляет поведение, используемое для выравнивания области шкалы времени по ширине страницы."
type: docs
weight: 3440
url: /ru/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Представляет поведение, используемое для выравнивания области шкалы времени по ширине страницы.

```csharp
public enum TimescaleFitBehavior
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DefinedInView | `0` | Раздел календаря отображается в соответствии со свойством View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage отображаемого представления. |
| NoScaleToEndDate | `1` | Раздел календаря отображается точно до EndDate, даже если на странице есть пустое пространство. |
| NoScaleToEndOfPage | `2` | Раздел календаря отображается до конца (правой стороны) последней страницы. Таким образом, последняя отображаемая дата может превышать EndDate. |
| ScaleToEndOfPage | `3` | Рендеринговый движок попытается выровнять даты так, чтобы EndDate был выровнен с концом (правой стороной) последней страницы. Соответствует включенной опции MS Project "Page Setup \ View \ Fit timescale to end of page". |

## Примеры

Показывает, как использовать TimescaleFitBehavior, чтобы шкала времени диаграммы Ганта соответствовала концу последней страницы.

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

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


