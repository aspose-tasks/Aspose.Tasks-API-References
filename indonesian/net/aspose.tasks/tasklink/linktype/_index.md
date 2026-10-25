---
title: "TaskLink.LinkType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur tipe tautan"
type: docs
weight: 60
url: /id/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Mendapatkan atau mengatur tipe tautan.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Contoh

Menampilkan cara mendapatkan/mengatur tipe tautan dari tautan tugas.

```csharp
var project = new Project();

// Tambahkan tugas baru
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Tautkan tugas dengan tipe tautan diatur ke Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Lihat Juga

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


