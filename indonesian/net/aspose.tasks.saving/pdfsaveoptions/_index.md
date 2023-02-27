---
title: PdfSaveOptions
second_title: Aspose.Tasks untuk Referensi .NET API
description: Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF.
type: docs
weight: 1860
url: /id/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Menginisialisasi instance baru dari`PdfSaveOptions`kelas yang dapat digunakan untuk menyimpan dokumen di[`PDF`](../savefileformat/) format. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Mendapat atau mengatur daftar instance dari[`BarStyle`](../../aspose.tasks.visualization/barstyle/) kelas yang muncul di tampilan proyek. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Mendapat atau menyetel tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Standarnya adalahPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Mendapat atau menetapkan ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname/) { get; set; } | Mendapat atau menyetel font default untuk rendering. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Mendapat atau menyetel detail tanda tangan digital. Jika tidak disetel, penandatanganan tidak akan dilakukan. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah waktu non-kerja harus diambil (Nilai defaultnya adalah TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Mendapat atau menyetel detail enkripsi. Jika tidak disetel, enkripsi tidak akan dilakukan. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Mendapat atau menetapkan tanggal untuk menyelesaikan rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah tinggi baris harus ditambah agar sesuai dengan kontennya. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Mendapat atau menyetel apakah bagian kalender dari tampilan harus dirender ke akhir (sisi kanan) halaman terakhir. Jika nilainya false, bagian kalender dirender tepat ke EndDate, meskipun ada ruang kosong di halaman. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback/) { get; set; } | Mendapat atau menyetel panggilan balik yang dapat digunakan untuk menyesuaikan font yang diselesaikan. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Mendapat atau menetapkan daftar[`Gridline`](../../aspose.tasks.visualization/gridline/) yang muncul di tampilan proyek. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah legenda harus ditampilkan pada setiap halaman (Nilai defaultnya adalah BENAR). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah tugas penting harus ditampilkan dalam warna merah (Nilai default adalah FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Mendapat atau menyetel warna waktu tidak bekerja. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Mendapat atau menetapkan jumlah halaman proyek. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Mendapat atau menyetel daftar nomor halaman untuk disimpan saat menyimpan tata letak proyek ke file terpisah. Semua halaman akan disimpan jika daftar ini kosong. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Mendapat atau menyetel panggilan balik yang ditentukan pengguna yang digunakan untuk mendapatkan aliran keluaran untuk setiap halaman yang dirender. Berlaku saat[`SaveToSeparateFiles`](./savetoseparatefiles/) opsi digunakan. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Mendapat atau mengatur ukuran halaman yang akan dirender (Nilai defaultnya adalah PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Mendapat atau menyetel[`PresentationFormat`](../saveoptions/presentationformat/) di mana dokumen akan disimpan. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah jarak antara tugas terakhir dan footer harus dikurangi. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah suatu proyek harus dirender ke satu halaman saat proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat di satu halaman. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah subtugas pada bilah tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada bilah Gantt subtugas akan digulung ke bilah tugas ringkasan. Untuk tugas ringkasan, Rollup bidang menunjukkan apakah bilah tugas ringkasan menampilkan bar yang digulung. Anda harus menyetel bidang Batal untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digulung ke sana. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Mendapat atau mengatur format penyimpanan dokumen jika objek opsi penyimpanan ini digunakan. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah akan menyimpan halaman proyek ke file terpisah. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Mendapat atau menyetel tanggal mulai rendering. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Mendapat atau menyetel pembanding untuk mengurutkan tugas di bagan Gantt dan bagan Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Mendapat atau menyetel kondisi yang digunakan untuk memfilter tugas yang diberikan pada bagan Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Mendapat atau menyetel jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Standarnya adalahFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Mendapat atau mengatur daftar instance dari[`TextStyle`](../../aspose.tasks.visualization/textstyle/) kelas yang muncul di tampilan proyek. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Mendapat atau menyetel[`Timescale`](../saveoptions/timescale/) nilai yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) ditampilkan saat proyek disimpan ke format grafis. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah sikat gradien harus digunakan saat merender Gantt Chart. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah font default harus digunakan untuk rendering. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Mendapat atau menyetel daftar kolom tampilan untuk dirender ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) . Jika tidak disetel maka id tugas, nama tugas, mulai dan selesai hanya akan dirender. Jika keduanya Lihat dan[`ViewSettings`](../saveoptions/viewsettings/)properti disetel, kolom dari View menimpa kolom dari ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Mendapat atau menyetel tampilan ([`View`](../saveoptions/view/) ) untuk merender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Gambar. Jika properti ini disetel,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) properti diabaikan saat proyek disimpan. Tampilan harus dari salah satu layar berikut (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, Lembar Tugas, Penggunaan Tugas, Lembar Sumber Daya, Penggunaan Sumber Daya) |

### Lihat juga

* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
