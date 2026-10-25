---
title: "SaveOptions.Timescale"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol etmek için kullanılan Timescale değerini alır veya ayarlar."
type: docs
weight: 200
url: /tr/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

`Timescale` değerini alır veya ayarlar; bu değer proje grafik formatında kaydedildiğinde zaman ölçeğinin (varsa) nasıl render edileceğini kontrol eder.

```csharp
public Timescale Timescale { get; set; }
```

## Örnekler

Render edilecek minimal zaman periyodunun nasıl ayarlanacağını gösterir. Varsayılan değer <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Tek sayfa görüntüsü olarak kaydet (Varsayılan olarak Timescale.days)
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// Tek sayfa görüntüsü olarak kaydet (Timescale.ThirdsOfMonths)
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// Tek sayfa görüntüsü olarak kaydet (Timescale.Months)
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

Kaydetme seçenekleri aracılığıyla zaman ölçeği katmanlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// Gantt Chart görünümünün zaman ölçeği katmanlarını ayarla
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// projeyi bir görüntü olarak kaydet
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

Görünüm ayarlarında tanımlanan zaman ölçeği ayarlarıyla görev kullanım görünümünün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// SaveOptions'ı tanımlayın ve TaskUsageView zaman ölçeği ayarlarının kullanılmasını belirtin.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

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

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


