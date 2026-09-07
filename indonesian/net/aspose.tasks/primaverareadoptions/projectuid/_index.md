---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraReadOptions. Mendapatkan atau mengatur UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek"
type: docs
weight: 30
url: /id/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Mendapatkan atau mengatur UID proyek yang akan dibaca dari file yang berisi beberapa proyek.

```csharp
public int ProjectUid { get; set; }
```

## Contoh

Menampilkan cara membaca proyek dari file Primavera XML atau Primavera XER yang berisi beberapa proyek.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Mengembalikan proyek dengan UID khusus
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


