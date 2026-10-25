---
title: "GanttChartView.GanttChartView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView yapıcı. GanttChartView sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

[`GanttChartView`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public GanttChartView()
```

## Örnekler

Zaman ölçeği katmanlarının nasıl değiştirileceğini gösterir.

```csharp
var project = new Project();

// Gantt Chart Görünümünü Başlat
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// Zaman Ölçeği sayısını ayarla
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

// Gantt Chart Görünümünü projeye ekle
project.Views.Add(view);

// projeye bazı test verileri ekle
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Zaman ölçeklerini, ayarladığımız zaman ölçeği ayarlarını (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) kullanarak renderlemek için 'Timescale.DefinedInView' seçeneğini kullanın.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### Ayrıca Bakınız

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


