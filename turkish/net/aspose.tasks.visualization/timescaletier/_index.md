---
title: "Sınıf TimescaleTier"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TimescaleTier sınıfı. Gantt Şeması'nda zaman ölçeğinin tek bir katmanını temsil eder"
type: docs
weight: 3450
url: /tr/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Gantt Çizelgesi üzerindeki zaman ölçeğinin tek bir katmanını temsil eder.

```csharp
public sealed class TimescaleTier
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | `TimescaleTier` sınıfının yeni bir örneğini başlatır. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | `TimescaleTier` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını alır veya ayarlar ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Katman için etiketlerin gösterileceği zaman birimi aralığını alır veya ayarlar. Varsayılan değer 1'dir. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Bu katmanda tarih işaretinin işlenmesi için bir geri çağırma işlevini alır veya ayarlar. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Zaman ölçeği katmanı için tarih etiketi [`DateLabel`](../datelabel/) alır veya ayarlar. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrağı alır veya ayarlar. Değer 'true' ise, zaman dilimi birden fazla sayfaya yayıldığında, dönem için tarih etiketleri her sayfada render edilir. Değer 'false' ise, tarih etiketi [`Alignment`](./alignment/) özelliğinin değerine göre yalnızca bir kez render edilir. |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Katmandaki zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Zaman ölçeği katmanı için zaman ölçeği birimini [`TimescaleUnit`](../timescaleunit/) alır veya ayarlar. Varsayılan değer [`Days`](../timescaleunit/) dir. |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Katman etiketlerinin mali yıla göre temellendirilip temellendirilmeyeceğini belirten bir değeri alır veya ayarlar. |

## Örnekler

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


