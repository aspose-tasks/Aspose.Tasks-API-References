---
title: "Enum GridlineType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.GridlineType. Jenis garis kisi"
type: docs
weight: 3110
url: /id/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Tipe garis kisi.

```csharp
public enum GridlineType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| GanttRow | `0` | Menunjukkan Gridline tipe baris gantt. |
| TopTierColumn | `1` | Menunjukkan Gridline tipe kolom tingkat atas. |
| BottomTierColumn | `2` | Menunjukkan Gridline tipe kolom tingkat bawah. |
| SheetRow | `3` | Menunjukkan Gridline tipe baris lembar. |
| SheetColumn | `4` | Menunjukkan Gridline tipe kolom lembar. |
| UsageRow | `5` | Menunjukkan Gridline tipe baris penggunaan. |
| UsageColumn | `6` | Menunjukkan Gridline tipe kolom penggunaan. |
| GanttTitleVertical | `7` | Menunjukkan tipe garis kisi vertikal judul Gantt. |
| GanttTitleHorizontal | `8` | Menunjukkan tipe garis kisi horizontal judul Gantt. |
| BarRows | `9` | Menunjukkan tipe garis kisi baris Bar. |
| GanttProjectStart | `10` | Menunjukkan tipe garis kisi mulai proyek Gantt. |
| GanttProjectFinish | `11` | Menunjukkan tipe garis kisi selesai proyek Gantt. |
| GanttStatusDate | `12` | Menunjukkan jenis garis kisi tanggal status Gantt. |
| GanttCurrentDate | `13` | Menunjukkan jenis garis kisi tanggal saat ini Gantt. |
| GanttPageBreaks | `14` | Menunjukkan jenis garis kisi pemisah halaman Gantt. |
| MiddleTierColumn | `15` | Menunjukkan jenis garis kisi kolom tingkat menengah. |

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


