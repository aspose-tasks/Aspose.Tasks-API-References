---
title: "Tsk.IsSummary"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas adalah tugas ringkasan"
type: docs
weight: 720
url: /id/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Menentukan apakah sebuah tugas adalah tugas ringkasan.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


