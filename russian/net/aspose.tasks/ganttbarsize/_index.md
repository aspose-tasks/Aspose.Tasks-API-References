---
title: "Перечисление GanttBarSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.GanttBarSize. Указывает высоту полосы в пунктах"
type: docs
weight: 700
url: /ru/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Указывает высоту полосы в пунктах.

```csharp
public enum GanttBarSize
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| BarSize6 | `0` | Размер полосы 6 пунктов. |
| BarSize8 | `1` | Размер полосы 8 пунктов. |
| BarSize10 | `2` | Размер полосы 10 пунктов. |
| BarSize12 | `3` | Размер полосы 12 пунктов. |
| BarSize14 | `4` | Размер полосы 14 пунктов. |
| BarSize18 | `5` | Размер полосы 18 пунктов. |
| BarSize24 | `6` | Размер полосы 24 пунктов. |

## Примеры

Показывает, как установить некоторые полезные свойства представления диаграммы Ганта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// установить значение, указывающее, округляются ли полосы до ближайшего дня
view.BarRounding = false;
// установить высоту, в пунктах, полос Ганта в диаграмме Ганта
view.BarSize = GanttBarSize.BarSize24;
// установить значение, указывающее, будут ли скрыты сводные полосы при раскрытии сводовой задачи
view.HideRollupBarsWhenSummaryExpanded = true;
// установить цвет нерабочего времени
view.NonWorkingTimeColor = Color.Azure;
// установить значение, указывающее, должны ли полосы на диаграмме Ганта быть свернуты
view.RollUpGanttBars = true;
// установить значение, указывающее, должны ли отображаться разрывы задач на диаграмме Ганта
view.ShowBarSplits = true;
// установить значение, указывающее, должны ли отображаться чертежи на диаграмме Ганта
view.ShowDrawings = true;
// установить процент для уменьшения или увеличения интервала между единицами на уровне шкалы времени
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


