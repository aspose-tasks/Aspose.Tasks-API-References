---
title: "Prj.Guid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. GUID proyek"
type: docs
weight: 360
url: /id/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

GUID proyek.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


