---
title: "Tsk.IsRollup"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah informasi tentang batang Gantt subtask akan digabungkan ke batang tugas ringkasan."
type: docs
weight: 690
url: /id/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Menentukan apakah informasi tentang bar Gantt subtugas akan digabungkan ke bar tugas ringkasan.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


