---
title: "Prj.RemoveFileProperties"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah semua properti file akan dihapus saat menyimpan"
type: docs
weight: 600
url: /id/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Menentukan apakah semua properti file akan dihapus saat menyimpan.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


