---
title: "Tsk.SubprojectName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Lokasi sumber dari subproyek"
type: docs
weight: 1070
url: /id/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

Lokasi sumber dari subproyek.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Contoh

Menampilkan cara membuat tugas subproyek.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Tambah tugas
var task = project.RootTask.Children.Add("Task 1");

// Mengatur tautan subproyek baru
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


