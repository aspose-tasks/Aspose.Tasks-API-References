---
title: "Kelas Gridline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.Gridline. Garis horizontal atau vertikal yang muncul di tampilan proyek"
type: docs
weight: 3100
url: /id/net/aspose.tasks.visualization/gridline/
---
## Gridline class

Garis horizontal atau vertikal yang muncul dalam tampilan proyek.

```csharp
public class Gridline
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Gridline](gridline/)() | Menginisialisasi instance baru dari kelas `Gridline`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Mendapatkan atau mengatur [`Color`](./color/) dari sebuah gridline. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Mendapatkan atau mengatur tipe gridline ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Mendapatkan atau mengatur [`LinePattern`](../linepattern/) dari sebuah gridline. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Mengembalikan nilai kode hash untuk instance kelas `Gridline`. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


