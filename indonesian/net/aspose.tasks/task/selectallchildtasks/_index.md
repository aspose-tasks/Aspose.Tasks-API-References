---
title: "Task.SelectAllChildTasks"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengumpulkan secara rekursif semua tugas anak dari tugas ini"
type: docs
weight: 1400
url: /id/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Mengumpulkan secara rekursif semua tugas anak dari tugas ini.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Nilai Kembali

Daftar tugas anak dari tugas ini.

## Contoh

Menunjukkan cara mengiterasi tugas anak.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


