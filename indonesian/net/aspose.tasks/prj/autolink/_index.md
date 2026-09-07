---
title: "Prj.Autolink"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah tugas yang disisipkan atau dipindahkan secara otomatis ditautkan"
type: docs
weight: 70
url: /id/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Menentukan apakah tugas yang disisipkan atau dipindahkan secara otomatis ditautkan.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


