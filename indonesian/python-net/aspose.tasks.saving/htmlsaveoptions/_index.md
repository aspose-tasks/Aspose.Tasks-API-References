---
title: "HtmlSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 20
url: /id/python-net/aspose.tasks.saving/htmlsaveoptions/
---

## HtmlSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke HTML.

Tipe HtmlSaveOptions menampilkan anggota berikut:
## Konstruktor
| Nama | Deskripsi |
| :- | :- |
| HtmlSaveOptions() | Menginisialisasi sebuah instance baru dari kelas [HtmlSaveOptions](/tasks/python-net/aspose.tasks.saving/htmlsaveoptions/) |
## Properti
| Nama | Deskripsi |
| :- | :- |
| save_format |  |
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
| use_gradient_brush | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek. |
| view | Mendapatkan atau mengatur daftar kolom tampilan yang akan dirender ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Jika tidak diatur maka hanya ID tugas, nama tugas, mulai, dan selesai yang dirender.<br/>            Jika baik View maupun properti [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) diatur, kolom dari View akan menggantikan kolom dari ViewSettings. |
| view_settings | Mendapatkan atau mengatur sebuah tampilan ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) untuk dirender. Anda dapat menggunakan opsi ini untuk secara eksplisit menentukan tampilan mana yang harus disimpan ke format PDF, HTML, atau Image.<br/>            Jika properti ini diatur, properti [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) diabaikan ketika proyek disimpan.<br/>            Tampilan harus berasal dari salah satu layar berikut (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Mendapatkan atau mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci). |
| render_to_single_page | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek harus dirender ke satu halaman<br/>            ketika proyek disimpan dalam format grafis.<br/>            Ukuran halaman akan diubah sehingga proyek yang dirender dapat muat dalam satu halaman. |
| css_style_prefix | Mendapatkan atau mengatur awalan gaya CSS. |
| font_settings | Menentukan pengaturan font yang digunakan saat merender tampilan proyek. |
| reduce_footer_gap | Mendapatkan atau mengatur nilai yang menunjukkan apakah jarak antara tugas terakhir dan footer harus dikurangi. |
| include_project_name_in_page_header | Mendapatkan atau mengatur nilai yang menunjukkan apakah nama proyek harus disertakan dalam header halaman HTML. |
| include_project_name_in_title | Mendapatkan atau mengatur nilai yang menunjukkan apakah nama proyek harus disertakan dalam judul HTML. |
| pages | Mendapatkan atau mengatur daftar nomor halaman yang akan disimpan saat merender tata letak proyek. |
| export_css | Mendapatkan atau mengatur cara CSS diekspor. |
| export_images | Mendapatkan atau mengatur cara gambar diekspor. |
| export_fonts | Mendapatkan atau mengatur cara font diekspor. |
| css_saving_callback | Mendapatkan atau mengatur callback yang dipanggil untuk membuat sumber daya yang menyimpan CSS. |
| font_saving_callback | Mendapatkan atau mengatur callback yang dipanggil untuk membuat sumber daya yang menyimpan font. |
| image_saving_callback | Mendapatkan atau mengatur callback yang dipanggil untuk membuat sumber daya yang menyimpan font. |
| font_face_types | Mendapatkan atau mengatur jenis font face. |
| page_saving_callback | Mendapatkan atau mengatur callback yang didefinisikan pengguna yang digunakan untuk memperoleh aliran output untuk setiap halaman yang dirender. |

### Lihat Juga

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

