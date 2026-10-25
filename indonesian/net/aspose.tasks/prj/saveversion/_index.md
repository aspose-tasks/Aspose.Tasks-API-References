---
title: "Prj.SaveVersion"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Versi Microsoft Office Project dari mana file proyek disimpan"
type: docs
weight: 620
url: /id/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

Versi Microsoft Office Project yang digunakan saat file proyek disimpan.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
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


