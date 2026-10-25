---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraReadOptions. Mendapatkan atau mengatur sebuah flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan"
type: docs
weight: 20
url: /id/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Mendapatkan atau mengatur flag yang menentukan apakah pengidentifikasi unik asli entitas harus dipertahankan.

```csharp
public bool PreserveUids { get; set; }
```

## Contoh

Menampilkan cara memuat proyek Primavera dengan Id yang ditentukan menggunakan &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// atur opsi pembacaan Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// bekerja dengan proyek...
```

### Lihat Juga

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


