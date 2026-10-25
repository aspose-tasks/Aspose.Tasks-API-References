---
title: "TimelineView.DisplayOverlapped"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TimelineView özelliği. Üst üste gelen görevlerin birden fazla satırda gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/timelineview/displayoverlapped/
---
## TimelineView.DisplayOverlapped property

Üst üste gelen görevlerin birden çok satırda görüntülenip görüntülenmeyeceğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool DisplayOverlapped { get; set; }
```

## Örnekler

&lt;see cref=\"Aspose.Tasks.TimelineView\" /&gt; ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// zaman çizelgesi görünümünü başlat
var view = new TimelineView();

// Zaman Çizelgesi görünümünde tarihlerin nasıl biçimlendirileceğini gösteren bir değeri ayarla.
view.DateFormat = DateFormat.DateDddDd;
// Üst üste gelen görevlerin birden çok satırda görüntülenip görüntülenmeyeceğini gösteren bir değeri ayarla.
view.DisplayOverlapped = true;
// Kaydırma ve yakınlaştırma kontrolünün gösterilip gösterilmeyeceğini belirten bir değeri ayarla.
view.ShowPanZoom = true;
// Zaman ölçeğinin gösterilip gösterilmeyeceğini belirten bir değeri ayarla.
view.ShowTimescale = true;
// Bugünü temsil eden bir satırın gösterilip gösterilmeyeceğini belirten bir değeri ayarla.
view.ShowToday = true;
// Zaman çizelgesinde görevi görüntülemek için kaç satır kullanılacağını belirten bir değeri ayarla.
view.TextLinesCount = 2;

// Üst üste gelen görevlerin birden çok satırda görüntülenip görüntülenmeyeceğini gösteren bir değeri al.
Console.WriteLine("Show Dates: " + view.ShowDates);

// görünümü projeye ekle
project.Views.Add(view);

// projeye bazı test verileri ekle
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


