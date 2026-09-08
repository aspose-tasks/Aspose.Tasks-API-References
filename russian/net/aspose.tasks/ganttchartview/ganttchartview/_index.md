---
title: "GanttChartView.GanttChartView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор GanttChartView. Инициализирует новый экземпляр класса GanttChartView"
type: docs
weight: 10
url: /ru/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

Инициализирует новый экземпляр класса [`GanttChartView`](../).

```csharp
public GanttChartView()
```

## Примеры

Показывает, как изменить уровни шкалы времени.

```csharp
var project = new Project();

// Инициализировать представление диаграммы Ганта
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// установить количество шкал времени
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// добавить представление диаграммы Ганта в проект
project.Views.Add(view);

// добавить некоторые тестовые данные в проект
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Используйте параметр 'Timescale.DefinedInView' для отрисовки шкал времени с использованием настроек шкалы времени, которые мы задали (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### См. также

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


