---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LoadOptions. Mendapatkan atau mengatur instance tertentu dari kelas PrimaveraReadOptions yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera Primavera P6 XER atau Primavera P6 Xml"
type: docs
weight: 60
url: /id/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Mendapatkan atau mengatur instance tertentu dari kelas [`PrimaveraReadOptions`](../../primaverareadoptions/) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


