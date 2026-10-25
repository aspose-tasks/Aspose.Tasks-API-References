---
title: "Sınıf ProgressLines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.ProgressLines sınıfı. Gantt Şeması görünümünde ilerleme çizgilerini temsil eder."
type: docs
weight: 3290
url: /tr/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Gantt Çizelgesi görünümündeki ilerleme çizgilerini temsil eder.

```csharp
public class ProgressLines
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProgressLines](progresslines/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | İlerleme çizgilerinin gösterileceği tarihi alır veya ayarlar. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Proje başlangıç tarihinin başından itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Tarih biçimini alır veya ayarlar ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Mevcut tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Tekrarlayan aralıklarla ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | İlerleme çizgi etiketi için kullanılan yazı tipini alır veya ayarlar. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Temel plan veya gerçek için ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Mevcut ilerleme çizgisi için çizgi rengini alır veya ayarlar. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Mevcut ilerleme çizgisinin çizgi desenini alır veya ayarlar. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Diğer ilerleme çizgisi rengini alır veya ayarlar. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Diğer ilerleme çizgisi için çizgi desenini alır veya ayarlar. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Diğer ilerleme noktasının rengini alır veya ayarlar. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Diğer ilerleme çizgisinin ilerleme nokta şeklini alır veya ayarlar. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | İlerleme noktasının rengini alır veya ayarlar. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | İlerleme nokta şeklini alır veya ayarlar. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Tekrarlayan aralığı alır veya ayarlar. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | İlerleme çizgileri için görüntülenecek seçilen tarihlerin listesini alır. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


