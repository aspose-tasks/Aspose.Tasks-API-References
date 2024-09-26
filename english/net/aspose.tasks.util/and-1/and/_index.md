---
title: And1.And
second_title: Aspose.Tasks for .NET API Reference
description: And constructor. Initializes a new instance of the And class
type: docs
weight: 10
url: /net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

Initializes a new instance of the [`And`](../) class.

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cond1 | ICondition`1 | First condition. |
| cond2 | ICondition`1 | Second condition. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


