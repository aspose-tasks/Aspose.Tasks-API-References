---
title: "ResourceAssignment.Delete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ResourceAssignment method. Menghapus penugasan sumber daya dari koleksi penugasan proyek"
type: docs
weight: 680
url: /id/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Menghapus penugasan sumber daya dari koleksi penugasan proyek.

```csharp
public void Delete()
```

## Contoh

Menampilkan cara menghapus penugasan sumber daya.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


