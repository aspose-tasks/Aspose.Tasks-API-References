---
title: "Class PrimaveraSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.PrimaveraSaveOptions. Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera XER"
type: docs
weight: 2150
url: /id/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Mengizinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Menginisialisasi instance baru dari kelas `PrimaveraSaveOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Mendapatkan atau mengatur kenaikan yang digunakan dalam penomoran ulang ID aktivitas. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Mendapatkan atau mengatur awalan yang digunakan dalam penomoran ulang ID aktivitas. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Mendapatkan atau mengatur akhiran yang digunakan dalam penomoran ulang ID aktivitas. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah perlu menomori ulang ID aktivitas. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |

## Contoh

Menampilkan cara bekerja dengan &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// buat opsi penyimpanan Primavera dan sesuaikan
var options = new PrimaveraSaveOptions
                  {
                      // tentukan awalan dan akhiran sebuah aktivitas
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // kontrol penomoran ulang aktivitas
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


