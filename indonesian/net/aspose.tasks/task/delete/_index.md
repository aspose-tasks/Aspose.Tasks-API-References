---
title: "Task.Delete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Menghapus sebuah tugas dari koleksi tugas proyek induk dan semua penugasannya"
type: docs
weight: 1320
url: /id/net/aspose.tasks/task/delete/
---
## Task.Delete method

Menghapus sebuah tugas dari koleksi tugas proyek induk dan semua penugasannya.

```csharp
public void Delete()
```

## Contoh

Menampilkan cara menghapus sebuah tugas.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// hapus sebuah tugas
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


