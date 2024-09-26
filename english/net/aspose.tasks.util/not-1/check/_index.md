---
title: Not1.Check
second_title: Aspose.Tasks for .NET API Reference
description: Not method. Returns true if the specified object satisfy the condition
type: docs
weight: 20
url: /net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Returns true if the specified object satisfy the condition.

```csharp
public bool Check(T el)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | T | The object to check. |

### Return Value

True if the object satisfy the condition.

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.Not`1" /&gt; condition.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // gather all project tasks
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // create a filter condition
    var filter = new NullCondition();

    // and reverse it by applying <see cref="Aspose.Tasks.Util.Not`1" /> condition
    var condition = new Not<Task>(filter);

    // apply the condition to the collected tasks
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### See Also

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


