---
title: "Prj.Manager"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Manajer sebuah proyek"
type: docs
weight: 450
url: /id/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

Manajer proyek.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Manager.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


