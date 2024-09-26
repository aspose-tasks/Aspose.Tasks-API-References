---
title: And1.Check
second_title: Aspose.Tasks for .NET API Reference
description: And method. Returns true if the specified object satisfy the conditions
type: docs
weight: 20
url: /net/aspose.tasks.util/and-1/check/
---
## And&lt;T&gt;.Check method

Returns true if the specified object satisfy the conditions.

```csharp
public bool Check(T el)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | T | The object to check. |

### Return Value

True if the object satisfy the conditions.

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.And`1" /&gt; condition.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // gather all project tasks
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // create a filter condition that filters summary tasks
    var condition1 = new SummaryCondition();

    // create a filter condition that filters not null tasks
    var condition2 = new NotNullCondition();

    // and join them by applying <see cref="Aspose.Tasks.Util.And`1" /> condition
    var joinedCondition = new And<Task>(condition1, condition2);

    // apply the condition to the collected tasks
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

        // work with other properties...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### See Also

* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


