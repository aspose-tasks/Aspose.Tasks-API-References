---
title: "Kelas HeaderFooterInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.HeaderFooterInfo. Mewakili konten visual header footer atau legenda yang digunakan untuk pencetakan dan rendering tampilan"
type: docs
weight: 3130
url: /id/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Mewakili konten visual header, footer, atau legenda yang digunakan untuk pencetakan \\ rendering tampilan.

```csharp
public class HeaderFooterInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Menginisialisasi instance baru dari kelas `HeaderFooterInfo`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Mendapatkan atau mengatur gambar terpusat yang akan ditampilkan dalam elemen induk. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar terpusat. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Mendapatkan atau mengatur teks terpusat untuk ditampilkan dalam elemen induk. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Mendapatkan atau mengatur gambar yang diratakan ke kiri untuk ditampilkan dalam elemen induk. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar kiri. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Mendapatkan atau mengatur teks yang diratakan ke kiri untuk ditampilkan dalam elemen induk. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Mendapatkan atau mengatur gambar yang diratakan ke kanan untuk ditampilkan dalam elemen induk. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Mendapatkan atau mengatur ukuran tampilan gambar kanan. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Mendapatkan atau mengatur teks yang diratakan ke kanan untuk ditampilkan dalam elemen induk. |

## Contoh

Menampilkan cara membaca informasi header/footer halaman.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


