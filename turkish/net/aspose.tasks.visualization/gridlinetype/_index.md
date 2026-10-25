---
title: "Enum GridlineType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.GridlineType enum. Gridline türü"
type: docs
weight: 3110
url: /tr/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Kılavuz çizgi türü.

```csharp
public enum GridlineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| GanttRow | `0` | Gantt satırı ızgara çizgi türünün ızgara çizgisini gösterir. |
| TopTierColumn | `1` | Üst seviye sütun ızgara çizgi türünün ızgara çizgisini gösterir. |
| BottomTierColumn | `2` | Alt seviye sütun ızgara çizgi türünün ızgara çizgisini gösterir. |
| SheetRow | `3` | Sayfa satırı ızgara çizgi türünün ızgara çizgisini gösterir. |
| SheetColumn | `4` | Sayfa sütunu ızgara çizgi türünün ızgara çizgisini gösterir. |
| UsageRow | `5` | Kullanım satırı ızgara çizgi türünün ızgara çizgisini gösterir. |
| UsageColumn | `6` | Kullanım sütunu ızgara çizgi türünün ızgara çizgisini gösterir. |
| GanttTitleVertical | `7` | Gantt başlığı dikey ızgara çizgi türünü gösterir. |
| GanttTitleHorizontal | `8` | Gantt başlığı yatay ızgara çizgi türünü gösterir. |
| BarRows | `9` | Çubuk satırları ızgara çizgi türünü gösterir. |
| GanttProjectStart | `10` | Gantt proje başlangıç ızgara çizgi türünü gösterir. |
| GanttProjectFinish | `11` | Gantt proje bitiş ızgara çizgi türünü gösterir. |
| GanttStatusDate | `12` | Gantt durum tarihi ızgara çizgi tipini gösterir. |
| GanttCurrentDate | `13` | Gantt geçerli tarih ızgara çizgi tipini gösterir. |
| GanttPageBreaks | `14` | Gantt sayfa sonları ızgara çizgi tipini gösterir. |
| MiddleTierColumn | `15` | Orta katman sütun ızgara çizgi tipinin ızgara çizgisini gösterir. |

## Örnekler

Izgara çizgileriyle çalışmayı görsel formatlarda kaydederken nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // ızgara çizgi tipini ayarla (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> bir ızgara çizgi için ayarla.
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


