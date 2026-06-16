---
title: Project.SelectAllChildTasks
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Recursively collects all child tasks of the root task
type: docs
weight: 1230
url: /net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Recursively collects all child tasks of the root task.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Return Value

The collection of tasks.

## Examples

Shows how to renumber selected tasks' WBS codes.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// output: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// output: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### See Also

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


