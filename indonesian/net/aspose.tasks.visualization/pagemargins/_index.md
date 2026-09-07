---
title: "Kelas PageMargins"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageMargins. Mewakili margin halaman untuk pencetakan"
type: docs
weight: 3230
url: /id/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Mewakili margin halaman untuk pencetakan.

```csharp
public class PageMargins
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageMargins](pagemargins/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Mendapatkan atau mengatur posisi tempat mencetak batas. Dapat menjadi salah satu nilai dari enumerasi [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Mendapatkan atau mengatur ukuran margin bawah dalam sentimeter. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Mendapatkan atau mengatur ukuran margin kiri dalam sentimeter. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Mendapatkan atau mengatur ukuran margin kanan dalam sentimeter. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Mendapatkan atau mengatur ukuran margin atas dalam sentimeter. |

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


