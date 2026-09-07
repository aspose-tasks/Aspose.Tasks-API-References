---
title: "PageMargins.Top"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "PageMargins properti. Mendapatkan atau mengatur ukuran margin atas dalam sentimeter"
type: docs
weight: 60
url: /id/net/aspose.tasks.visualization/pagemargins/top/
---
## PageMargins.Top property

Mendapatkan atau mengatur ukuran margin atas dalam sentimeter.

```csharp
public double Top { get; set; }
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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


