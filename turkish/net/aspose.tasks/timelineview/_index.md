---
title: "Sınıf TimelineView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TimelineView sınıfı. Bir projenin zaman çizelgesi görünümünü temsil eder"
type: docs
weight: 2580
url: /tr/net/aspose.tasks/timelineview/
---
## TimelineView class

Bir projenin zaman çizelgesi görünümünü temsil eder.

```csharp
public class TimelineView : View
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TimelineView](timelineview/)() | `TimelineView` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Zaman Çizelgesi görünümünde tarihlerin nasıl biçimlendirileceğini gösteren bir değeri alır veya ayarlar. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Üst üste gelen görevlerin birden çok satırda görüntülenip görüntülenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Tek bir görünümde kullanılan bir filtreyi alır veya ayarlar. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Tek bir görünümün grubunu alır veya ayarlar. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamayacağını belirten bir değeri alır veya ayarlar. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Bir View nesnesinin adını alır veya ayarlar. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](../view/pageinfo/) sınıfının bir örneğini alır. mpp dosya formatında bulunan sayfa ayarı verilerini temsil eder. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View nesnesinin üst nesnesini alır. Salt okunur [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Tek bir görünüm için ekran tipini alır. Salt okunur [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Tarihlerin gösterilip gösterilmeyeceğini belirten bir değeri alır. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project'in tek bir görünüm adını Şerit'teki Görünüm veya Diğer Görünümler açılır listelerinde gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Kaydırma ve yakınlaştırma kontrolünün gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Zaman ölçeğinin gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Bugünü temsil eden bir satırın gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Tek bir görünümün tablosunu alır veya ayarlar. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Zaman çizelgesinde görevi görüntülemek için kaç satır kullanılacağını belirten bir değeri alır veya ayarlar. |
| [Type](../../aspose.tasks/view/type/) { get; } | Tek bir görünümdeki öğenin türünü alır, örneğin görevler veya kaynaklar. Salt okunur [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Bir görünümün benzersiz tanımlayıcısını alır. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Görünümdeki [`OleObject`](../oleobject/) yerleşimini ve görünümünü temsil eden nesneler koleksiyonunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Mevcut örneği aynı türdeki başka bir nesneyle karşılaştırır ve mevcut örneğin diğer nesneye göre sıralama düzeninde önce mi, sonra mı yoksa aynı konumda mı olduğunu belirten bir tam sayı döndürür. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) sınıfının örneği için bir karma kod değeri döndürür. |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


