---
title: "Aspose::Tasks::Saving::SaveOptions kelas"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks untuk C++"
description: "Ini adalah kelas dasar abstrak untuk kelas-kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke dalam format tertentu."
type: docs
weight: 10
url: /id/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Ini adalah kelas dasar abstrak untuk kelas-kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek ke dalam format tertentu.

Sebuah instance dari kelas turunan apa pun dari kelas SaveOptions diteruskan ke overload Save berbasis stream atau string Save agar pengguna dapat menentukan opsi khusus saat menyimpan dokumen.

## Metode

| Nama | Deskripsi |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Mendapatkan daftar instance dari kelas BarStyle yang muncul dalam tampilan proyek. |
| [get_CustomPageSize](./get_custompagesize/) | Mendapatkan ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Mendapatkan nilai yang menunjukkan apakah waktu non‑kerja harus digambar (Nilai default adalah TRUE). |
| [get_EndDate](./get_enddate/) | Mendapatkan tanggal untuk menyelesaikan rendering. |
| [get_FitContent](./get_fitcontent/) | Mendapatkan nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Mendapatkan apakah bagian kalender dari tampilan harus dirender hingga akhir (sisi kanan) halaman terakhir. Jika nilai false, bagian kalender dirender tepat hingga EndDate, meskipun ada ruang kosong pada halaman. |
| [get_Gridlines](./get_gridlines/) | Mendapatkan daftar Gridline yang muncul dalam tampilan proyek. |
| [get_IsPortrait](./get_isportrait/) | Mendapatkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Mendapatkan nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Mendapatkan array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Mendapatkan nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Mendapatkan warna waktu non‑kerja. |
| [get_PageCount](./get_pagecount/) | Mendapatkan jumlah halaman proyek. |
| [get_PageSize](./get_pagesize/) | Mendapatkan ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Mendapatkan PresentationFormat di mana dokumen akan disimpan. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Mendapatkan nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Mendapatkan nilai yang menunjukkan apakah subtugas pada batang tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digabungkan ke batang tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah batang tugas ringkasan menampilkan batang yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan menjadi Yes agar subtugas apa pun dapat digabungkan ke dalamnya. |
| [get_StartDate](./get_startdate/) | Mendapatkan tanggal untuk memulai rendering. |
| [get_TextStyles](./get_textstyles/) | Mendapatkan daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [get_Timescale](./get_timescale/) | Mendapatkan nilai Timescale yang digunakan untuk mengontrol cara timescale (jika ada) dirender ketika proyek disimpan ke format grafis. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Mendapatkan perilaku yang menentukan cara menyelaraskan ujung kanan timescale dengan ujung halaman. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Mendapatkan nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [get_View](./get_view/) | Mendapatkan daftar kolom tampilan yang akan dirender ( GanttChartColumn ). Jika tidak disetel, maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender. Jika properti View dan ViewSettings keduanya disetel, kolom dari View akan menggantikan kolom dari ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Mendapatkan tampilan ( View ) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini disetel, properti Visualization::PresentationFormat diabaikan saat proyek disimpan. Tampilan harus berasal dari salah satu layar berikut (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| [set_BarStyles](./set_barstyles/) | Menetapkan daftar instance kelas BarStyle yang muncul dalam tampilan proyek. |
| [set_CustomPageSize](./set_custompagesize/) | Menetapkan ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Menetapkan nilai yang menunjukkan apakah waktu non‑kerja harus digambar (Nilai default adalah TRUE). |
| [set_EndDate](./set_enddate/) | Menetapkan tanggal untuk menyelesaikan proses rendering. |
| [set_FitContent](./set_fitcontent/) | Menetapkan nilai yang menunjukkan apakah tinggi baris harus ditingkatkan agar sesuai dengan isinya. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Menetapkan apakah bagian kalender dari tampilan harus dirender hingga akhir (sisi kanan) halaman terakhir. Jika nilai false, bagian kalender dirender tepat sampai EndDate, meskipun ada ruang kosong pada halaman. |
| [set_Gridlines](./set_gridlines/) | Menetapkan daftar Gridline yang muncul dalam tampilan proyek. |
| [set_IsPortrait](./set_isportrait/) | Menetapkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Menetapkan nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Menetapkan array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman. Jika null, item default akan dirender. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Menetapkan nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Menetapkan warna waktu non‑kerja. |
| [set_PageSize](./set_pagesize/) | Menetapkan ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Menetapkan PresentationFormat di mana dokumen akan disimpan. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Menetapkan nilai yang menunjukkan apakah proyek harus dirender ke satu halaman ketika proyek disimpan dalam format grafis. Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Menetapkan nilai yang menunjukkan apakah subtugas pada batang tugas rangkuman harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digabungkan ke batang tugas rangkuman. Untuk tugas rangkuman, bidang Rollup menunjukkan apakah batang tugas rangkuman menampilkan batang yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas rangkuman menjadi Yes agar subtugas apa pun dapat digabungkan ke dalamnya. |
| [set_StartDate](./set_startdate/) | Menetapkan tanggal untuk memulai rendering. |
| [set_TextStyles](./set_textstyles/) | Menetapkan daftar gaya teks yang diterapkan selama rendering tampilan proyek. |
| [set_Timescale](./set_timescale/) | Menetapkan nilai Timescale yang digunakan untuk mengontrol cara timescale (jika ada) dirender ketika proyek disimpan ke format grafis. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Menetapkan perilaku yang menentukan cara menyelaraskan ujung kanan timescale dengan ujung halaman. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Menetapkan nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| [set_View](./set_view/) | Menetapkan daftar kolom tampilan yang akan dirender ( GanttChartColumn ). Jika tidak disetel, maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender. Jika properti View dan ViewSettings keduanya disetel, kolom dari View akan menggantikan kolom dari ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Menetapkan tampilan ( View ) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image. Jika properti ini disetel, properti Visualization::PresentationFormat diabaikan saat proyek disimpan. Tampilan harus berasal dari salah satu layar berikut (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

