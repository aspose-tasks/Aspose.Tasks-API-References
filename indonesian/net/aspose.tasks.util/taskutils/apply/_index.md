---
title: "TaskUtils.Apply"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskUtils. Menerapkan algoritma yang ditentukan ke setiap tugas dalam pohon."
type: docs
weight: 10
url: /id/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Menerapkan algoritma yang ditentukan ke setiap tugas dalam pohon.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | Tugas | Akar pohon |
| alg | ITreeAlgorithm`1 | Algoritma yang diterapkan. |
| tingkat | Int32 | Level tugas akar. |

## Contoh

Menunjukkan cara bekerja dengan algoritma pohon.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// mengumpulkan semua tugas proyek
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// bekerja dengan tugas seperti daftar biasa
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


