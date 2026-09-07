---
title: "Project.TaskLinks"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan objek TaskLinkCollection"
type: docs
weight: 930
url: /id/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Mendapatkan objek [`TaskLinkCollection`](../../tasklinkcollection/).

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Contoh

Menampilkan cara membuat tautan tugas.

```csharp
var project = new Project();

// Tambahkan tugas baru
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Tautkan tugas
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### Lihat Juga

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


