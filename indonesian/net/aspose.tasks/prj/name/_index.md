---
title: "Prj.Name"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Nama proyek"
type: docs
weight: 540
url: /id/net/aspose.tasks/prj/name/
---
## Prj.Name field

Nama proyek.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Contoh

Menunjukkan cara membaca/menulis nama proyek.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


