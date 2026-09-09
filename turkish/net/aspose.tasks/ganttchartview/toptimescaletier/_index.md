---
title: "GanttChartView.TopTimescaleTier"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Görünümün üst zaman ölçeği katmanının ayarlarını alır veya ayarlar. TimescaleTier"
type: docs
weight: 190
url: /tr/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

Görünümün üst zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
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

Zaman ölçeği katman etiketlerini nasıl özelleştireceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Görev bağlantılarını ekle
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// zaman ölçeği katmanlarını ayarla

// üst katmanı ayarla
// Gantt Şeması görünümünün üst zaman ölçeği katmanını ayarla.
view.MiddleTimescaleTier = new TimescaleTier();
// Zaman ölçeği katmanı için zaman ölçeği birimini <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> ayarla.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// Katman için etiketlerin gösterileceği zaman birimi aralığını ayarla.
view.MiddleTimescaleTier.Count = 1;
// Zaman ölçeği katmanı için tarih etiketini <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> ayarla.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ayarla (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// katmanda zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değer ayarlayın.
view.MiddleTimescaleTier.ShowTicks = true;
// katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değer ayarlayın.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// daha iyi görselleştirme için eklendi
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// orta katman tarihlerini özelleştirin
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Görünümde tanımlanan zaman ölçeği ayarlarını (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) kullanarak zaman ölçeklerini oluşturmak için 'Timescale.DefinedInView' seçeneğini kullanın.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Ayrıca Bakınız

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


