---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraReadOptions. Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER"
type: docs
weight: 50
url: /id/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


