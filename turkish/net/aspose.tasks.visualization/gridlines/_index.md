---
title: "Class Gridlines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.Gridlines class. GanttChart görünümünde görülen ızgara çizgilerini temsil eder."
type: docs
weight: 3120
url: /tr/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

GanttChart görünümünde görünen ızgara çizgilerini temsil eder.

```csharp
public class Gridlines
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Gridlines](gridlines/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Izgara çizgileri arasındaki aralığı belirten 0 ile 99 arasındaki sayıyı alır veya ayarlar. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | İkincil ızgara çizgilerinin rengini alır veya ayarlar. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | İkincil ızgara çizgileri için çizgi desenini alır veya ayarlar. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Normal ızgara çizgilerinin rengini alır veya ayarlar. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Normal ızgara çizgileri için çizgi desenini alır veya ayarlar. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


