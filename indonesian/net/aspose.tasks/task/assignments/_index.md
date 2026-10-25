---
title: "Task.Assignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan koleksi penugasan sumber daya untuk objek ini"
type: docs
weight: 120
url: /id/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Mendapatkan koleksi penugasan sumber daya untuk objek ini.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Contoh

Menampilkan cara mengiterasi penugasan tugas.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // tampilkan penugasan tugas
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Lihat Juga

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


