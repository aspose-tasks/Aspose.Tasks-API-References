---
title: "Prj.NewTasksAreManual"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah tugas baru dibuat secara manual"
type: docs
weight: 550
url: /id/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Menentukan apakah tugas baru dibuat secara manual.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


