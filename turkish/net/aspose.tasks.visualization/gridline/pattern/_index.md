---
title: "Gridline.Pattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Gridline özelliği. Bir ızgara çizgisinin LinePattern'ını alır veya ayarlar."
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

Bir ızgara çizgisinin [`LinePattern`](../../linepattern/) değerini alır veya ayarlar.

```csharp
public LinePattern Pattern { get; set; }
```

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

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


