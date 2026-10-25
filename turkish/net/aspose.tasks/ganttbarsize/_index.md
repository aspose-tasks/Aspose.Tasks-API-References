---
title: "GanttBarSize enum'ı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GanttBarSize enum. Bir çubuğun yüksekliğini puan cinsinden belirtir"
type: docs
weight: 700
url: /tr/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Bir çubuğun yüksekliğini puan cinsinden belirtir.

```csharp
public enum GanttBarSize
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| BarSize6 | `0` | Çubuk boyutu 6 puan. |
| BarSize8 | `1` | Çubuk boyutu 8 puan. |
| BarSize10 | `2` | Bar boyutu 10 puan. |
| BarSize12 | `3` | Bar boyutu 12 puan. |
| BarSize14 | `4` | Bar boyutu 14 puan. |
| BarSize18 | `5` | Bar boyutu 18 puan. |
| BarSize24 | `6` | Bar boyutu 24 puan. |

## Örnekler

Gantt şema görünümünün bazı faydalı özelliklerini nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// çubukların en yakın güne yuvarlanıp yuvarlanmayacağını belirten bir değer ayarla
view.BarRounding = false;
// Gantt Şeması'ndaki Gantt çubuklarının yüksekliğini, puan cinsinden ayarla
view.BarSize = GanttBarSize.BarSize24;
// özet görevi genişletirken toplama çubuklarının gizlenip gizlenmeyeceğini belirten bir değer ayarla
view.HideRollupBarsWhenSummaryExpanded = true;
// çalışma dışı zaman rengini ayarla
view.NonWorkingTimeColor = Color.Azure;
// Gantt Şeması'ndaki çubukların toplanıp toplanmayacağını belirten bir değer ayarla
view.RollUpGanttBars = true;
// Gantt Şeması'ndaki görev bölünmelerinin gösterilip gösterilmeyeceğini belirten bir değer ayarla
view.ShowBarSplits = true;
// Gantt Şeması'ndaki çizimlerin gösterilip gösterilmeyeceğini belirten bir değer ayarla
view.ShowDrawings = true;
// zaman ölçeği katmanındaki birimler arasındaki boşluğu azaltmak veya büyütmek için bir yüzde ayarla
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


