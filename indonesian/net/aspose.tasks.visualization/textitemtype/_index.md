---
title: "Enum TextItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.TextItemType. Tipe item untuk mengubah gaya teks"
type: docs
weight: 3410
url: /id/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Jenis item untuk mengubah gaya teks.

```csharp
public enum TextItemType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| RowColumnTitles | `0` | Judul baris dan kolom. |
| CriticalTasks | `1` | Tugas kritis. |
| NoncriticalTasks | `2` | Tugas nonkritikal. |
| MilestoneTasks | `3` | Tugas tonggak. |
| InactiveTasks | `4` | Tugas tidak aktif. |
| SummaryTasks | `5` | Tugas ringkasan. |
| AssignmentRow | `6` | Baris penugasan. |
| TopTimescaleTier | `7` | Tingkat skala waktu atas. |
| BottomTimescaleTier | `8` | Tingkat skala waktu bawah. |
| MiddleTimescaleTier | `9` | Tingkat skala waktu tengah. |
| Resources | `10` | Lembar sumber daya. |
| OverallocatedResources | `11` | Sumber daya yang dialokasikan berlebih. |
| TaskFilterHighlight | `12` | Item teks Sorotan Filter Tugas. |
| BarTextBottom | `13` | Item teks Bar Bawah. |
| BarTextInside | `14` | Item teks Bar Dalam. |
| BarTextLeft | `15` | Item teks Bar Kiri. |
| BarTextRight | `16` | Item teks Bar Kanan. |
| BarTextTop | `17` | Item teks Bar Atas. |
| MarkedTasks | `18` | Item teks tugas yang ditandai. |
| ProjectSummary | `19` | Item teks tugas ringkasan proyek. |
| ExternalTasks | `20` | Item teks tugas eksternal. |
| Allocated | `21` | Item teks yang dialokasikan. |
| ChangedCells | `22` | Sel yang diubah. |

## Contoh

Menunjukkan cara bekerja dengan tipe item teks.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


