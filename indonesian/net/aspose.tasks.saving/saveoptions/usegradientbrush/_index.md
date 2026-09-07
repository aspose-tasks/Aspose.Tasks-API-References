---
title: "SaveOptions.UseGradientBrush"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart"
type: docs
weight: 220
url: /id/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Mendapatkan atau mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Catatan

Hanya berlaku ketika tampilan diagram Gantt dirender.

## Contoh

menunjukkan cara mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


