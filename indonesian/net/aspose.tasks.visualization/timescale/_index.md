---
title: "Enum Timescale"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.Timescale. Mendefinisikan opsi yang menentukan cara merender skala waktu dalam tampilan Penggunaan Tugas Diagram Gantt atau Penggunaan Sumber Daya ketika proyek diekspor ke format grafis."
type: docs
weight: 3430
url: /id/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Mendefinisikan opsi yang menentukan bagaimana cara merender skala waktu dalam tampilan Gantt Chart, Task Usage, atau Resource Usage ketika proyek diekspor ke format grafis.

```csharp
public enum Timescale
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| DefinedInView | `0` | Gunakan pengaturan skala waktu yang didefinisikan dalam properti tampilan proyek: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Berlaku untuk format yang berisi data tampilan. Misalnya, proyek yang dibaca dari format MPP. |
| Days | `1` | Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu hari. |
| ThirdsOfMonths | `10` | Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail adalah sepertiga bulan. |
| Months | `30` | Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu bulan. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


