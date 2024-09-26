---
title: TaskUtils.Find
second_title: Aspose.Tasks for .NET API Reference
description: TaskUtils method. Finds a task which satisfy the condition in a tree of tasks
type: docs
weight: 30
url: /net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Finds a task which satisfy the condition in a tree of tasks.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parameter | Type | Description |
| --- | --- | --- |
| root | Task | Root of the tree. |
| cond | ICondition`1 | Applied condition. |

### Return Value

Task if task was found, otherwise null.

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; method.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // builds new tree of tasks which satisfy the condition 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

    // gather tasks from a tree
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // iterate over plain list of tasks 
    // which durations are greater or equal than 2 working days
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Returns true if the specified object satisfy the conditions.
    /// </summary>
    /// <param name="el">The object to check.</param>
    /// <returns>True if the object satisfy the conditions.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### See Also

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


