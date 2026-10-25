---
title: "Task.OutlineOutdent"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mempromosikan tugas dalam outline"
type: docs
weight: 1390
url: /id/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Menaikkan tingkat tugas dalam outline.

```csharp
public void OutlineOutdent()
```

## Contoh

Menampilkan cara mengurangi indentasi tugas.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// kurangi indentasi tugas
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


