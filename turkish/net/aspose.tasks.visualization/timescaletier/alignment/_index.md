---
title: "TimescaleTier.Alignment"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TimescaleTier özelliği. Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını HorizontalStringAlignment alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/timescaletier/alignment/
---
## TimescaleTier.Alignment property

Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ([`HorizontalStringAlignment`](../../horizontalstringalignment/)) alır veya ayarlar.

```csharp
public HorizontalStringAlignment Alignment { get; set; }
```

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

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


