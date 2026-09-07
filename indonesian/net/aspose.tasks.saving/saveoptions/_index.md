---
title: "Kelas SaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.SaveOptions. Ini adalah kelas dasar abstrak untuk kelas-kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke format tertentu."
type: docs
weight: 2190
url: /id/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

Ini adalah kelas dasar abstrak untuk kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke format tertentu.

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Mendapatkan atau mengatur daftar instance dari kelas [`BarStyle`](../../aspose.tasks.visualization/barstyle/) yang muncul dalam tampilan proyek. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Mendapatkan atau mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah waktu non‑kerja harus digambar (Nilai default adalah TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Mendapatkan atau mengatur tanggal untuk menyelesaikan rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Mendapatkan atau mengatur daftar [`Gridline`](../../aspose.tasks.visualization/gridline/) yang muncul dalam tampilan proyek. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Mendapatkan atau mengatur nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Mendapatkan atau mengatur array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Mendapatkan atau mengatur warna waktu non‑kerja. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Mendapatkan atau mengatur jumlah halaman proyek. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Mendapatkan atau mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Mendapatkan atau mengatur [`PresentationFormat`](./presentationformat/) di mana dokumen akan disimpan. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah subtugas pada batang tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digabungkan ke batang tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah batang tugas ringkasan menampilkan batang yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke dalamnya. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Mendapatkan atau mengatur tanggal mulai merender. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Mendapatkan atau mengatur daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Mendapatkan atau mengatur nilai [`Timescale`](./timescale/) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender saat proyek disimpan ke format grafis. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Mendapatkan atau mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan yang akan dirender ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Jika tidak diatur, maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender. Jika properti View dan [`ViewSettings`](./viewsettings/) keduanya diatur, kolom dari View akan menggantikan kolom dari ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Mendapatkan atau mengatur tampilan ([`View`](./view/)) yang akan dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini diatur, properti [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) akan diabaikan saat proyek disimpan. Tampilan harus berasal dari salah satu layar berikut (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Catatan

Sebuah instance dari kelas turunan apa pun dari kelas SaveOptions diteruskan ke overload Save aliran atau Save string agar pengguna dapat menentukan opsi khusus saat menyimpan dokumen.

## Contoh

Menampilkan cara mengatur opsi apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Atur opsi fit content menjadi true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


