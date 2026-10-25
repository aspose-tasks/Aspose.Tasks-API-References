---
title: "Task.OutlineIndent"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Memberi indentasi pada tugas dalam outline"
type: docs
weight: 1380
url: /id/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Memberi indent pada tugas dalam outline.

```csharp
public void OutlineIndent()
```

## Contoh

Menunjukkan cara mengindentasi tugas.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// indentasi tugas
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


