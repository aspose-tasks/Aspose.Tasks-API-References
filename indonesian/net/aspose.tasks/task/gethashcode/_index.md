---
title: "Task.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengembalikan nilai kode hash untuk Task ini"
type: docs
weight: 1350
url: /id/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Mengembalikan nilai kode hash untuk Task ini.

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah tugas.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// kode hash dari sebuah tugas didasarkan pada uid dan nama tugas
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


