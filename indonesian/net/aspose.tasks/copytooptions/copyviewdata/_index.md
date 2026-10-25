---
title: "CopyToOptions.CopyViewData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CopyToOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah data tampilan harus disalin saat menyalin data proyek. Nilai default adalah true"
type: docs
weight: 20
url: /id/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Mendapatkan atau mengatur nilai yang menunjukkan apakah data tampilan harus disalin saat menyalin data proyek. Nilai default adalah true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


