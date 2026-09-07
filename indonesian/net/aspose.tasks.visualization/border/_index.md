---
title: "Enum Border"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.Border. Menentukan jenis batas."
type: docs
weight: 2970
url: /id/net/aspose.tasks.visualization/border/
---
## Border enumeration

Menentukan tipe batas.

```csharp
public enum Border
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| NoBorder | `0` | Tidak ada batas. |
| AroundEveryPage | `1` | Di sekitar setiap halaman. |
| OutsidePages | `2` | Pada halaman luar. |

## Contoh

Menampilkan cara bekerja dengan margin halaman.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// memungkinkan memodifikasi tampilan default
var margins = project.DefaultView.PageInfo.Margins;

// memungkinkan memodifikasi margin
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


