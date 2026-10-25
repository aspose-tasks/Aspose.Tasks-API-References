---
title: "GanttChartView.TimescaleSizePercentage"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği."
type: docs
weight: 180
url: /tr/net/aspose.tasks/ganttchartview/timescalesizepercentage/
---
## GanttChartView.TimescaleSizePercentage property

```csharp
public ushort TimescaleSizePercentage { get; set; }
```

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


