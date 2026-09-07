---
title: "Prj.LastSaved"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal ketika proyek disimpan terakhir kali. Disimpan dalam format UTC di file mpp. Tipe DateTime"
type: docs
weight: 440
url: /id/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

Tanggal ketika proyek terakhir disimpan. Disimpan dalam format UTC di file mpp. Tipe DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
```

## Contoh

Menampilkan cara memeriksa versi penyimpanan proyek dan tanggal penyimpanan.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Tampilkan versi proyek
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


