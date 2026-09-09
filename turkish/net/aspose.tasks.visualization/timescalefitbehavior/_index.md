---
title: "Enum TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior enum. Zaman ölçeği alanını sayfa genişliğiyle hizalamak için kullanılan bir davranışı temsil eder."
type: docs
weight: 3440
url: /tr/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Zaman ölçeği alanını sayfa genişliğiyle hizalamak için kullanılan bir davranışı temsil eder.

```csharp
public enum TimescaleFitBehavior
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DefinedInView | `0` | Takvim bölümü, oluşturulan Görünüm'ün View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage özelliğine göre işlenir. |
| NoScaleToEndDate | `1` | Takvim bölümü, bir sayfada boş alan olsa bile, EndDate'e tam olarak işlenir. |
| NoScaleToEndOfPage | `2` | Takvim bölümü, son sayfanın sonuna (sağ tarafına) işlenir. Böylece son işlenen tarih EndDate'i aşabilir. |
| ScaleToEndOfPage | `3` | İşleme motoru, tarihleri EndDate'in son sayfanın sonuna (sağ tarafına) hizalanacak şekilde hizalamaya çalışır. Bu, MS Project'in "Sayfa Ayarı \ Görünüm \ Zaman ölçeğini sayfanın sonuna sığdır" seçeneğinin etkin olmasına karşılık gelir. |

## Örnekler

TimescaleFitBehavior'ı kullanarak Gantt şemasının zaman ölçeğini son sayfanın sonuna sığdırmayı gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


