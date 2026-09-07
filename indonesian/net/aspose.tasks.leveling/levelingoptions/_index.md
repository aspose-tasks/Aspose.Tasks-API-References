---
title: "Kelas LevelingOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Leveling.LevelingOptions. Memungkinkan untuk menentukan parameter penyeimbangan sumber daya"
type: docs
weight: 940
url: /id/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Memungkinkan untuk menentukan parameter perataan sumber daya.

```csharp
public sealed class LevelingOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Menginisialisasi instance baru dari kelas `LevelingOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Mendapatkan atau mengatur token yang dapat digunakan untuk membatalkan operasi penyeimbangan proyek. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Mendapatkan atau mengatur tanggal akhir periode penyeimbangan. Nilai default adalah tanggal selesai proyek. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Mendapatkan urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih. Setelah menentukan tugas yang menyebabkan alokasi berlebih dan tugas mana yang dapat ditunda, urutan yang ditentukan digunakan untuk menentukan tugas mana yang harus ditunda pertama. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Mendapatkan atau mengatur callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Mendapatkan atau mengatur tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama penyeimbangan sumber daya. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Mendapatkan atau mengatur daftar sumber daya yang akan diseimbangkan. Jika disetel null, semua sumber daya proyek akan diseimbangkan. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Mendapatkan atau mengatur tanggal mulai periode penyeimbangan. Nilai default adalah tanggal mulai proyek. |

## Contoh

Menampilkan cara menyeimbangkan sumber daya tertentu, menyesuaikan opsi penyeimbangan, dan memeriksa pesan algoritma penyeimbangan.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


