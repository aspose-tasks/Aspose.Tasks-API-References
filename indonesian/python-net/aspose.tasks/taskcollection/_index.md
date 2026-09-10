---
title: "TaskCollection"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 1140
url: /id/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Mewakili kumpulan [Task](/tasks/python-net/aspose.tasks/task/) objek.

Tipe TaskCollection menampilkan anggota-anggota berikut:
## Properti
| Nama | Deskripsi |
| :- | :- |
| parent_project | Mendapatkan proyek induk dari objek TaskCollection. |
## Methods
| Nama | Deskripsi |
| :- | :- |
| add() | Tambahkan tugas yang ditentukan ke instance kelas [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Jika ParentProject.CalculationMode bernilai None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang-bidang yang bergantung seperti slack, pekerjaan dan biaya, id, serta tingkat outline).<br/>            Jika ParentProject.CalculationMode bernilai Manual, metode ini akan menghitung hanya id tugas, tingkat outline, dan nomor outline secara otomatis.<br/>            Jika ParentProject.CalculationMode bernilai Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis<br/>            (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, pekerjaan dan biaya, menghitung ulang id dan tingkat outline). |
| add(task_name) | Menambahkan tugas baru ke koleksi tugas anak. |
| add(task_name, before_task_id) |  |
| add(parameters) | Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama. |
| to_list() | Mengonversi objek TaskCollection menjadi daftar objek [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Mengembalikan tugas dengan Uid yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini . |
| get_by_id(id) | Mengembalikan tugas dengan Id yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini . |

### Lihat Juga

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

