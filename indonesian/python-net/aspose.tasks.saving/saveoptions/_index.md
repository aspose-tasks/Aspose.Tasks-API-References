---
title: "SaveOptions"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 130
url: /id/python-net/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

Ini adalah kelas dasar abstrak untuk kelas yang memungkinkan pengguna menentukan opsi tambahan saat menyimpan proyek<br/>            ke format tertentu.

Tipe SaveOptions menampilkan anggota-anggota berikut:
## Properti
| Nama | Deskripsi |
| :- | :- |
| save_format | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| bar_styles | Mendapatkan atau mengatur daftar instance dari kelas [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) yang muncul dalam tampilan proyek. |
| draw_non_working_time | Mendapatkan atau mengatur nilai yang menunjukkan apakah waktu non-kerja harus digambar (Nilai default adalah TRUE). |
| end_date | Mendapatkan atau mengatur tanggal untuk menyelesaikan rendering. |
| timescale_fit_behavior | Mendapatkan atau mengatur perilaku yang menentukan bagaimana menyelaraskan ujung kanan skala waktu dengan ujung halaman. |
| fit_content | Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris harus ditingkatkan untuk menyesuaikan isinya. |
| gridlines | Mendapatkan atau mengatur daftar [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) yang muncul dalam tampilan proyek. |
| legend_drawing_options | Mendapatkan atau mengatur nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage. |
| legend_items | Mendapatkan atau mengatur array PageLegendItem yang menentukan batang mana yang harus dirender dalam legenda halaman.<br/>            Jika null, item default akan dirender. |
| mark_critical_tasks | Mendapatkan atau mengatur nilai yang menunjukkan apakah tugas kritis harus ditampilkan dengan warna merah (Nilai default adalah FALSE). |
| non_working_time_color | Mendapatkan atau mengatur warna waktu non‑kerja. |
| page_count | Mendapatkan atau mengatur jumlah halaman proyek. |
| page_size | Mendapatkan atau mengatur ukuran halaman yang akan dirender (Nilai default adalah PageSize.A4). |
| is_portrait | Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| presentation_format | Mendapatkan atau mengatur [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) di mana dokumen akan disimpan. |
| roll_up_gantt_bars | Mendapatkan atau mengatur nilai yang menunjukkan apakah subtugas pada batang tugas ringkasan harus ditandai.<br/>            Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digulung ke batang tugas ringkasan.<br/>            Untuk tugas ringkasan, bidang Rollup menunjukkan apakah batang tugas ringkasan menampilkan batang yang telah digulung.<br/>            Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Yes agar subtugas apa pun dapat digulung ke mereka. |
| start_date | Mendapatkan atau mengatur tanggal mulai merender. |
| text_styles | Mendapatkan atau mengatur daftar gaya teks yang diterapkan selama merender tampilan proyek. |
| timescale | Mendapatkan atau mengatur nilai [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) yang digunakan untuk mengontrol bagaimana skala waktu (jika ada) dirender ketika proyek disimpan ke format grafis. |
| use_gradient_brush | Mendapatkan atau mengatur nilai yang menunjukkan apakah kuas gradien harus digunakan saat merender Gantt Chart. |
| view | Mendapatkan atau mengatur daftar kolom tampilan yang akan dirender ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Jika tidak diatur maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender.<br/>            Jika baik View maupun properti [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) diatur, kolom dari View akan menggantikan kolom dari ViewSettings. |
| view_settings | Mendapatkan atau mengatur sebuah tampilan ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image.<br/>            Jika properti ini diatur, properti [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) diabaikan ketika proyek disimpan.<br/>            Tampilan harus berasal dari salah satu layar berikut (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Mendapatkan atau mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| render_to_single_page | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek harus dirender ke satu halaman<br/>            ketika proyek disimpan dalam format grafis.<br/>            Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |

### Lihat Juga

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

