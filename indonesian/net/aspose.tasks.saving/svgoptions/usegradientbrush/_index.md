---
title: "SvgOptions.UseGradientBrush"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "SvgOptions properti. Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek. Saat ini penggunaan kuas gradien tidak didukung untuk merender ke SVG"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek. Saat ini penggunaan kuas gradien tidak didukung untuk merender ke SVG.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Contoh

Menampilkan cara menyimpan proyek sebagai file SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // atur <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> di mana dokumen akan disimpan
                            PresentationFormat = PresentationFormat.GanttChart,

                            // atur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya
                            FitContent = true,

                            // atur periode waktu minimal untuk merender. Nilai default adalah <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek
                            // Saat ini penggunaan kuas gradien tidak didukung untuk merender ke SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Lihat Juga

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


