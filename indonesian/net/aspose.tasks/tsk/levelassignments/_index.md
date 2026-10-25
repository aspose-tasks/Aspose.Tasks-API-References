---
title: "Tsk.LevelAssignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah fungsi leveling dapat menunda dan membagi penugasan individu untuk menyelesaikan alokasi berlebih."
type: docs
weight: 750
url: /id/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Menentukan apakah fungsi leveling dapat menunda dan membagi penugasan individu untuk menyelesaikan alokasi berlebih.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


