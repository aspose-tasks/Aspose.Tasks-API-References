---
title: "Gridline.Gridline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor Gridline. Menginisialisasi instance baru dari kelas Gridline."
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

Menginisialisasi instance baru dari kelas [`Gridline`](../).

```csharp
public Gridline()
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


