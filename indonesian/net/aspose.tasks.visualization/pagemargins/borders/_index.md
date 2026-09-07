---
title: "PageMargins.Borders"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "PageMargins properti. Mendapatkan atau mengatur posisi tempat mencetak batas. Bisa menjadi salah satu nilai dari enumerasi Border"
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Mendapatkan atau mengatur posisi tempat mencetak batas. Bisa menjadi salah satu nilai dari enumerasi [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
```

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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


