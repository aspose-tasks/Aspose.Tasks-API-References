---
title: "GanttChartView.ProgressLines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Chart görünümü için ilerleme çizgilerini alır veya ayarlar. ProgressLines"
type: docs
weight: 120
url: /tr/net/aspose.tasks/ganttchartview/progresslines/
---
## GanttChartView.ProgressLines property

Gantt Chart görünümü için ilerleme çizgilerini alır veya ayarlar. `ProgressLines`.

```csharp
public ProgressLines ProgressLines { get; set; }
```

## Örnekler

İlerleme çizgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// İlerleme çizgisini tanımlayalım
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// İlerleme çizgilerinin gösterileceği tarihi ayarla. Bir projenin durum tarihini ayarlayalım.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// Proje başlangıç tarihinden itibaren ilerleme çizgilerinin gösterilip gösterilmeyeceğini belirten bir değer ayarla
progressLines.BeginAtProjectStart = true;
// Tarih formatını ayarla (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// Mevcut tarihte ilerleme çizgisinin gösterilip gösterilmeyeceğini belirten bir değer ayarla.
progressLines.DisplayAtCurrentDate = true;
// Tekrarlayan aralıklarla ilerleme çizgisinin gösterilip gösterilmeyeceğini belirten bir değer ayarla.
progressLines.DisplayAtRecurringIntervals = true;
// Seçilen tarihlerde ilerleme çizgilerinin gösterilip gösterilmeyeceğini belirten bir değer ayarla
progressLines.DisplaySelected = true;
// Temel plan için mi yoksa gerçek için mi ilerleme çizgilerinin gösterilip gösterilmeyeceğini belirten bir değer ayarla.
progressLines.IsBaselinePlan = false;
// İlerleme çizgi etiketi için kullanılan yazı tipini ayarla.
progressLines.Font = new FontDescriptor("Arial", 10);
// Mevcut ilerleme çizgisi için çizgi rengini ayarla.
progressLines.LineColor = Color.Aquamarine;
// Mevcut ilerleme çizgisinin çizgi desenini ayarla.
progressLines.LinePattern = LinePattern.Dashed;
// Diğer ilerleme çizgisi rengini ayarla.
progressLines.OtherLineColor = Color.Azure;
// Diğer ilerleme çizgisi için çizgi desenini ayarla.
progressLines.OtherLinePattern = LinePattern.Dotted;
// Diğer ilerleme noktasının rengini ayarla.
progressLines.OtherProgressPointColor = Color.Red;
// Diğer ilerleme çizgisinin ilerleme noktasının şeklini ayarla.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// İlerleme noktasının rengini ayarla.
progressLines.ProgressPointColor = Color.Orange;
// ilerleme noktası şeklini ayarla.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// yinelenen aralığı ayarla.
progressLines.RecurringInterval = new RecurringInterval();
// yinelenen aralığı ayarla.
progressLines.RecurringInterval.Interval = Interval.Daily;
// günlük gün numarasını ayarla
progressLines.RecurringInterval.DailyDayNumber = 1;
// her ilerleme satırı için tarihi gösterip göstermeyeceğini belirten bir değeri ayarla.
progressLines.ShowDate = true;

// ilerleme satırlarını kontrol edelim
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [ProgressLines](../../../aspose.tasks.visualization/progresslines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


