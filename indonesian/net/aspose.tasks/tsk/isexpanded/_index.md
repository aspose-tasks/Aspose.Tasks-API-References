---
title: "Tsk.IsExpanded"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah tugas ringkasan diperluas atau tidak dalam tampilan GanttChart"
type: docs
weight: 590
url: /id/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Menentukan apakah tugas ringkasan diperluas atau tidak dalam tampilan GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


