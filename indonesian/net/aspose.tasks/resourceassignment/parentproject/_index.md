---
title: "ResourceAssignment.ParentProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceAssignment. Mendapatkan proyek induk untuk penugasan ini"
type: docs
weight: 420
url: /id/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Mendapatkan proyek induk untuk penugasan ini.

```csharp
public Project ParentProject { get; }
```

## Contoh

Menampilkan cara menggunakan proyek induk dari penugasan sumber daya.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// atur durasi penugasan dengan menggunakan tipe unit waktu proyek default.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Lihat Juga

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


