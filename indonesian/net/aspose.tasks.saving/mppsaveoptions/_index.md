---
title: "Kelas MPPSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.MPPSaveOptions. Memungkinkan untuk menentukan opsi tambahan saat menyimpan data proyek ke MPP"
type: docs
weight: 2050
url: /id/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Mengizinkan untuk menentukan opsi tambahan saat menyimpan data proyek ke MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Menginisialisasi sebuah instance baru dari kelas `MPPSaveOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Mendapatkan atau mengatur kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. Saat ini didukung untuk format MS Project 2010 dan yang lebih baru. Nilai null menunjukkan bahwa file proyek tidak dilindungi. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP. MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Atur flag ini ke true untuk menghapusnya saat menyimpan. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menulis data filter saat menyimpan proyek ke format MPP. Data filter mencakup koleksi Project.TaskFilters dan Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menulis data grup saat menyimpan proyek ke format MPP. Data grup mencakup koleksi Project.TaskGroups dan Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan memperbarui data makro VBA yang ada dalam file MPP. Saat ini penulisan VbaModule.SourceCode didukung. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menulis data tampilan saat menyimpan proyek ke format MPP. Data tampilan mencakup koleksi Project.Views, Filters, dan Tables. |

## Contoh

Menampilkan cara menyimpan proyek ke dalam stream sebagai file MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // buat opsi penyimpanan
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // mengatur nilai yang menunjukkan apakah akan menghapus penugasan sumber daya tidak valid saat menyimpan ke MPP
        RemoveInvalidAssignments = true
    };

    // simpan MPP dengan opsi
    project.Save(stream, options);
}
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


