---
title: "Tsk.IsPublished"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Menentukan apakah tugas saat ini harus dipublikasikan ke Project Server bersama dengan sisa proyek"
type: docs
weight: 660
url: /id/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Menentukan apakah tugas saat ini harus dipublikasikan ke Project Server bersama dengan seluruh proyek.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


