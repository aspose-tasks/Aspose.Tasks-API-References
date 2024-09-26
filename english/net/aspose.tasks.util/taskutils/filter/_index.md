---
title: TaskUtils.Filter
second_title: Aspose.Tasks for .NET API Reference
description: TaskUtils method. Builds new tree of tasks which satisfy the condition
type: docs
weight: 20
url: /net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Builds new tree of tasks which satisfy the condition.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parameter | Type | Description |
| --- | --- | --- |
| root | Task | Root of the tree. |
| cond | ICondition`1 | Applied condition. |

### Return Value

Root of a new tree.

## Examples

Shows how to work with a condition.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // builds new tree of tasks which satisfy the condition 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

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

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Returns true if the specified object satisfy the conditions.
    /// </summary>
    /// <param name="el">The object to check.</param>
    /// <returns>True if the object satisfy the conditions.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### See Also

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


