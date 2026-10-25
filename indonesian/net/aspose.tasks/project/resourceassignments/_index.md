---
title: "Project.ResourceAssignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan objek ResourceAssignmentCollection"
type: docs
weight: 750
url: /id/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Mendapatkan objek ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Contoh

Menampilkan cara bekerja dengan penugasan sumber daya.

```csharp
var project = new Project();

// Tambahkan tugas dan sumber daya baru
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Tetapkan sumber daya ke tugas yang diinginkan
project.ResourceAssignments.Add(task, resource);
```

### Lihat Juga

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


