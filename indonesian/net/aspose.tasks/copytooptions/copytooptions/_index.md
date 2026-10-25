---
title: "CopyToOptions.CopyToOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor CopyToOptions. Menginisialisasi sebuah instance baru dari kelas CopyToOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Menginisialisasi sebuah instance baru dari kelas [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


