---
title: "Tsk.IsSubproject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas adalah proyek yang disisipkan"
type: docs
weight: 700
url: /id/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Menentukan apakah sebuah tugas adalah proyek yang disisipkan.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


