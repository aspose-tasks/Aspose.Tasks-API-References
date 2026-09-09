---
title: "Gridlines.Type"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Gridlines özelliği. Izgara çizgisi tipini alır veya ayarlar"
type: docs
weight: 70
url: /tr/net/aspose.tasks.visualization/gridlines/type/
---
## Gridlines.Type property

Izgara çizgi tipini alır veya ayarlar.

```csharp
public GridlineType Type { get; set; }
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

* enum [GridlineType](../../gridlinetype/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


