---
title: TaskCollection
second_title: Aspose.Tasks untuk Referensi .NET API
description: Merupakan kumpulan dariTask./task/ objek.
type: docs
weight: 2100
url: /id/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Merupakan kumpulan dari[`Task`](../task/) objek.

```csharp
public class TaskCollection : IList<Task>
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Mendapat jumlah objek yang terkandung dalam TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Mendapat nilai yang menunjukkan apakah koleksi ini hanya bisa dibaca. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Mendapat proyek induk dari objek TaskCollection. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Menambahkan tugas baru untuk memproyeksikan kumpulan tugas pada tingkat kerangka yang sama dari tugas terakhir. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada level kerangka yang sama. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Menambahkan tugas baru ke koleksi tugas anak. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Tambahkan tugas yang ditentukan ke instance dari`TaskCollection`class. Jika ParentProject.CalculationMode adalah Tidak ada, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwal ulang semua tugas proyek (tanggal mulai/selesai, menetapkan tanggal awal/akhir) dan menghitung bidang dependen seperti slacks, work dan kolom biaya, id, dan level garis besar). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, level garis besar, dan angka garis besar secara otomatis. Jika ParentProject.CalculationMode adalah Otomatis, metode ini menjadwal ulang semua tugas proyek secara otomatis (mulai/selesai tanggal, menetapkan tanggal awal/terlambat, menghitung kelonggaran, bidang pekerjaan dan biaya, menghitung ulang id dan tingkat kerangka). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Menambahkan tugas berulang baru ke koleksi tugas anak-anak. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Memeriksa apakah koleksi berisi item tertentu. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Mengembalikan tugas dengan ID tertentu yang leluhurnya adalah tugas induk dari koleksi ini . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Mengembalikan tugas dengan Uid tertentu yang leluhurnya adalah tugas induk dari koleksi ini . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Ini adalah implementasi stub dari metode Insert IList, yang hanya melempar NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Ini adalah implementasi rintisan dari metode Remove ICollection, yang hanya melempar NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Mengubah objek TaskCollection menjadi daftar[`Task`](../task/) objek. |

### Lihat juga

* class [Task](../task/)
* ruang nama [Aspose.Tasks](../../aspose.tasks/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
