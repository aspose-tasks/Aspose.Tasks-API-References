---
title: "GanttChartView.BarRounding"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "GanttChartView свойство. Получает или задает значение, указывающее, округляются ли полосы до ближайшего дня. Значение по умолчанию — True"
type: docs
weight: 30
url: /ru/net/aspose.tasks/ganttchartview/barrounding/
---
## GanttChartView.BarRounding property

Получает или задает значение, указывающее, округляются ли полосы до ближайшего дня. Значение по умолчанию: True.

```csharp
public bool BarRounding { get; set; }
```

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


