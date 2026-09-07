---
title: "Tsk.IsExternalTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas bersifat eksternal"
type: docs
weight: 600
url: /id/net/aspose.tasks/tsk/isexternaltask/
---
## Tsk.IsExternalTask field

Menentukan apakah sebuah tugas eksternal.

```csharp
public static readonly Key<bool, TaskKey> IsExternalTask;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsExternalTask.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExternalTask, true);

Console.WriteLine("Is External Task: " + task.Get(Tsk.IsExternalTask));
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


