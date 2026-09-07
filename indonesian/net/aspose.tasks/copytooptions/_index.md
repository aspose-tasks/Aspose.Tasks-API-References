---
title: "Kelas CopyToOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.CopyToOptions. Memungkinkan untuk menentukan opsi tambahan saat menyalin data proyek"
type: docs
weight: 340
url: /id/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Memungkinkan untuk menentukan opsi tambahan saat menyalin data proyek.

```csharp
public class CopyToOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Menginisialisasi instance baru dari kelas `CopyToOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah data tampilan harus disalin saat menyalin data proyek. Nilai default adalah true. |

## Contoh

Menampilkan cara menggunakan opsi penyalinan proyek.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// lewati penyalinan data tampilan saat menyalin data proyek umum.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


