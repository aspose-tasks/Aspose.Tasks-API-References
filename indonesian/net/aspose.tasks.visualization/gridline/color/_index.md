---
title: "Gridline.Color"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Gridline. Mendapatkan atau mengatur Color dari sebuah gridline."
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/gridline/color/
---
## Gridline.Color property

Mendapatkan atau mengatur `Color` dari sebuah gridline.

```csharp
public Color Color { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan garis kisi saat menyimpan dalam format visual.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // atur jenis garis kisi (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // atur <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> dari sebuah garis kisi
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Lihat Juga

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


