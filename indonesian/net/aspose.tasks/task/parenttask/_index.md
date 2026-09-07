---
title: "Task.ParentTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan tugas induk dari sebuah tugas"
type: docs
weight: 940
url: /id/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Mendapatkan tugas induk dari sebuah tugas.

```csharp
public Task ParentTask { get; }
```

## Contoh

Menampilkan cara menggunakan tugas induk dari sebuah tugas.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


