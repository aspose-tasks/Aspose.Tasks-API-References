---
title: "TaskLink.CrossProjectName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur proyek pendahulu eksternal"
type: docs
weight: 10
url: /id/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

Mendapatkan atau mengatur proyek pendahulu eksternal.

```csharp
public string CrossProjectName { get; set; }
```

## Contoh

Menampilkan cara menemukan tautan tugas lintas proyek.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Periksa tautan tugas lintas proyek
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


