---
title: "PageLegend.Width"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageLegend. Mendapatkan atau mengatur lebar bagian kiri yang berisi nama proyek dan tanggal secara default pada legenda dalam sentimeter"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Mendapatkan atau mengatur lebar bagian kiri (yang berisi nama dan tanggal proyek secara default) dari legenda dalam sentimeter.

```csharp
public double Width { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Saat mencoba mengatur ke nilai kurang dari 0. |

## Contoh

Menampilkan cara bekerja dengan informasi legenda halaman.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// mari membaca informasi legenda halaman
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// modifikasi legenda juga didukung
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


