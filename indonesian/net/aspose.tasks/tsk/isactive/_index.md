---
title: "Tsk.IsActive"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Menentukan apakah sebuah tugas aktif. Tugas tidak aktif tidak lagi memengaruhi tugas lain atau jadwal Proyek secara keseluruhan"
type: docs
weight: 550
url: /id/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Menentukan apakah sebuah tugas aktif. Tugas tidak aktif tidak lagi memengaruhi tugas lain atau jadwal Proyek secara keseluruhan.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


