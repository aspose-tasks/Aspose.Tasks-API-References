---
title: "Task.ParentProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan proyek induk dari sebuah tugas"
type: docs
weight: 930
url: /id/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Mendapatkan proyek induk dari sebuah tugas.

```csharp
public Project ParentProject { get; }
```

## Catatan

Panggil Project.UpdateReferences untuk memperbarui properti ini.

## Contoh

Menampilkan cara menggunakan proyek induk dari tugas.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// atur durasi untuk tugas dengan menggunakan tipe unit waktu proyek default.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Lihat Juga

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


