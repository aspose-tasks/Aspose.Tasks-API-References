---
title: "XamlOptions.XamlOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor XamlOptions. Menginisialisasi instance baru dari kelas XamlOptions yang dapat digunakan untuk menyimpan proyek dalam format XAML"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Menginisialisasi instance baru dari kelas [`XamlOptions`](../) yang dapat digunakan untuk menyimpan proyek dalam format XAML.

```csharp
public XamlOptions()
```

## Contoh

Menampilkan cara menyimpan proyek dalam format XAML dengan menggunakan opsi penyimpanan.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Lihat Juga

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


