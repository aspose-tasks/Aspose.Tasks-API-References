---
title: "Tsk.ExternalId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Jika sebuah tugas adalah tugas eksternal, ia berisi Id eksternal tugas tersebut"
type: docs
weight: 360
url: /id/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Jika sebuah tugas adalah tugas eksternal, ia berisi Id eksternal tugas tersebut.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Contoh

Menunjukkan cara mengidentifikasi tugas lintas proyek.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Tampilkan ID tugas dalam proyek eksternal
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Tampilkan ID tugas dalam proyek asli
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
```

Menunjukkan cara membuat tautan tugas lintas proyek - tautan ke tugas di proyek lain (eksternal).

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Untuk membuat tautan ke tugas dari proyek lain, kita harus membuat
// duplikatnya (atau "eksternal") tugas di proyek saat ini.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


