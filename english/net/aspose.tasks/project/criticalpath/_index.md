---
title: Project.CriticalPath
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. This is an On operation where n is the number of tasks in the project
type: docs
weight: 180
url: /net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. This is an O(n) operation, where n is the number of tasks in the project.

```csharp
public TaskCollection CriticalPath { get; }
```

### Return Value

a collection which represents a list of all critical tasks.

## Examples

Shows how to calculate a critical path of the project.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Display the critical path now
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### See Also

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


