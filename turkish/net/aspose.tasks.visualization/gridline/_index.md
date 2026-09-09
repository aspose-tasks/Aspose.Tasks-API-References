---
title: "Sınıf Gridline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.Gridline sınıfı. Proje görünümünde görünen yatay veya dikey çizgi"
type: docs
weight: 3100
url: /tr/net/aspose.tasks.visualization/gridline/
---
## Gridline class

Proje görünümünde görünen yatay veya dikey çizgi.

```csharp
public class Gridline
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Gridline](gridline/)() | Yeni bir `Gridline` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Alır veya ayarlar [`Color`](./color/) bir ızgara çizgisinin. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Alır veya ayarlar ızgara çizgisinin tipini ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Alır veya ayarlar [`LinePattern`](../linepattern/) bir ızgara çizgisinin. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | `Gridline` sınıfının örneği için bir karma kod değeri döndürür. |

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


