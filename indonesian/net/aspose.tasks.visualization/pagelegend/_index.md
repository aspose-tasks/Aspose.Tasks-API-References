---
title: "Kelas PageLegend"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageLegend. Mewakili legenda halaman yang digunakan untuk pencetakan proyek."
type: docs
weight: 3210
url: /id/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Mewakili legenda halaman yang digunakan untuk pencetakan proyek.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageLegend](pagelegend/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Mendapatkan atau mengatur gambar terpusat yang akan ditampilkan dalam elemen induk. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar terpusat. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Mendapatkan atau mengatur teks terpusat untuk ditampilkan dalam elemen induk. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Mendapatkan atau mengatur gambar yang diratakan ke kiri untuk ditampilkan dalam elemen induk. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar kiri. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Mendapatkan atau mengatur teks yang diratakan ke kiri untuk ditampilkan dalam elemen induk. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Mendapatkan atau mengatur halaman tempat legenda muncul. Dapat menjadi salah satu nilai dari enumerasi [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Mendapatkan atau mengatur gambar yang diratakan ke kanan untuk ditampilkan dalam elemen induk. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar kanan. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Mendapatkan atau mengatur teks yang diratakan ke kanan untuk ditampilkan dalam elemen induk. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Mendapatkan atau mengatur lebar bagian kiri (yang berisi nama dan tanggal proyek secara default) dari legenda dalam sentimeter. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


