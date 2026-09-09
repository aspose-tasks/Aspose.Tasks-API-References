---
title: "GanttChartView.Gridlines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Chart görünümünün Gridlines listesini alır veya ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

Gantt Chart görünümünün `Gridlines` listesini alır veya ayarlar.

```csharp
public List<Gridlines> Gridlines { get; set; }
```

## Örnekler

Izgara çizgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// Görünümün ilk ızgara çizgisini ayarlamaya izin verir.
var gridlines = view.Gridlines[0];
// Izgara çizgileri arasındaki aralığı belirten 0 ile 99 arasındaki sayıyı ayarlayın.
gridlines.Interval = 2;
// İkincil ızgara çizgilerinin rengini ayarlayın.
gridlines.IntervalColor = Color.Red;
// İkincil ızgara çizgileri için çizgi desenini ayarlayın
gridlines.IntervalPattern = LinePattern.Solid;
// Normal ızgara çizgilerinin rengini ayarlayın
gridlines.NormalColor = Color.Blue;
// Normal ızgara çizgileri için çizgi desenini ayarlayın
gridlines.NormalPattern = LinePattern.CloseDot;
// Izgara çizgi tipini ayarlayın
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


