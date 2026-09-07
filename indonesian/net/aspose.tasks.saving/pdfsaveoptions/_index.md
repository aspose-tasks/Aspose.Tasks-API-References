---
title: "Kelas PdfSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.PdfSaveOptions. Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF"
type: docs
weight: 2130
url: /id/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Mengizinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Menginisialisasi instance baru dari kelas `PdfSaveOptions` yang dapat digunakan untuk menyimpan dokumen dalam format [`PDF`](../savefileformat/). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Mendapatkan atau mengatur daftar instance dari kelas [`BarStyle`](../../aspose.tasks.visualization/barstyle/) yang muncul dalam tampilan proyek. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Mendapatkan atau mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Defaultnya adalah Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Mendapatkan atau mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Mendapatkan atau mengatur detail tanda tangan digital. Jika tidak diatur, maka tidak akan ada penandatanganan yang dilakukan. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah waktu non‑kerja harus digambar (Nilai default adalah TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Mendapatkan atau mengatur detail enkripsi. Jika tidak diatur, maka tidak akan ada enkripsi yang dilakukan. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Mendapatkan atau mengatur tanggal untuk menyelesaikan rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | Menentukan pengaturan font yang digunakan saat merender tampilan proyek. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Mendapatkan atau mengatur daftar [`Gridline`](../../aspose.tasks.visualization/gridline/) yang muncul dalam tampilan proyek. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Mendapatkan atau mengatur nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Mendapatkan atau mengatur array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Mendapatkan atau mengatur warna waktu non‑kerja. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Mendapatkan atau mengatur jumlah halaman proyek. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. Berlaku ketika opsi [`SaveToSeparateFiles`](./savetoseparatefiles/) digunakan. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Mendapatkan atau mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Mendapatkan atau mengatur [`PresentationFormat`](../saveoptions/presentationformat/) di mana dokumen akan disimpan. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah subtugas pada batang tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digabungkan ke batang tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah batang tugas ringkasan menampilkan batang yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke dalamnya. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman proyek akan disimpan ke file terpisah. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Mendapatkan atau mengatur tanggal mulai merender. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Mendapatkan atau mengatur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Defaultnya adalah Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Mendapatkan atau mengatur daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Mendapatkan atau mengatur nilai [`Timescale`](../saveoptions/timescale/) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Mendapatkan atau mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan yang akan dirender ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Jika tidak diatur, maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender. Jika properti View dan [`ViewSettings`](../saveoptions/viewsettings/) keduanya diatur, kolom dari View akan menggantikan kolom dari ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Mendapatkan atau mengatur tampilan ([`View`](../saveoptions/view/)) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Gambar. Jika properti ini diatur, properti [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) diabaikan saat proyek disimpan. Tampilan harus berasal dari salah satu layar berikut (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## Contoh

Menampilkan cara menyimpan halaman terpilih dari sebuah proyek ke file PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// mari periksa jumlah halaman yang dapat diekspor
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


