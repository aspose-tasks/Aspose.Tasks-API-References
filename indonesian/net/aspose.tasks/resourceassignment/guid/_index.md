---
title: "ResourceAssignment.Guid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceAssignment. Mendapatkan atau mengatur pengidentifikasi unik untuk penugasan ini"
type: docs
weight: 290
url: /id/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Mendapatkan atau mengatur pengidentifikasi unik untuk penugasan ini.

```csharp
public Guid? Guid { get; set; }
```

## Contoh

Menampilkan cara membaca GUID penugasan sumber daya.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


