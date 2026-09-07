---
title: "Tsk.IsManual"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas dijadwalkan secara manual"
type: docs
weight: 610
url: /id/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Menentukan apakah sebuah tugas dijadwalkan secara manual.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


