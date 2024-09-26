---
title: RemoveTask.Alg
second_title: Aspose.Tasks for .NET API Reference
description: RemoveTask method. Do nothing
type: docs
weight: 20
url: /net/aspose.tasks.util/removetask/alg/
---
## RemoveTask.Alg method

Do nothing.

```csharp
public void Alg(Task el, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | Task | Object to process. |
| level | Int32 | Tree node level. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


