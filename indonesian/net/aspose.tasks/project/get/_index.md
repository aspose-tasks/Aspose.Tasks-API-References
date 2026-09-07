---
title: "Project.Get"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini"
type: docs
weight: 1080
url: /id/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parameter | Deskripsi |
| --- | --- |
| T | tipe nilai yang dipetakan. |
| key | kunci properti yang ditentukan. [`Prj`](../../prj/) untuk mendapatkan kunci properti. |

### Nilai Kembali

nilai yang dipetakan ke properti dalam wadah ini.

## Contoh

Menampilkan cara memeriksa versi proyek.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Tampilkan versi proyek
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


