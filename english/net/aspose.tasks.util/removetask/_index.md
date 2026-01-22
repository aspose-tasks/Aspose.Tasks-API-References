---
title: Class RemoveTask
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.RemoveTask class. Removes the specified task from a tree of tasks
type: docs
weight: 2730
url: /net/aspose.tasks.util/removetask/
---
## RemoveTask class

Removes the specified task from a tree of tasks.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Constructors

| Name | Description |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Initializes a new instance of the `RemoveTask` class. |

## Methods

| Name | Description |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Do nothing. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Do nothing. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Removes the task from the specified parent task. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.RemoveTask" /&gt; tree based algorithm.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // use tree based algorithm to delete task1 from the tree
    var algorithm = new RemoveTask(task1);

    // apply the algorithm to the task tree
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // check the results
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### See Also

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


