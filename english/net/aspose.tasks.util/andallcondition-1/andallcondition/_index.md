---
title: AndAllCondition1.AndAllCondition
second_title: Aspose.Tasks for .NET API Reference
description: AndAllCondition constructor. Initializes a new instance of the AndAllCondition class
type: docs
weight: 10
url: /net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Initializes a new instance of the [`AndAllCondition`](../) class.

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| conditions | List`1 | The list of conditions. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.AndAllCondition`1" /&gt; condition.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // gather all project tasks
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // create a filter condition that filters not null tasks
                             new NotNullCondition(),

                             // create a filter condition that filters summary tasks
                             new SummaryCondition()
                         };

    // and join them by applying <see cref="Aspose.Tasks.Util.AndAllCondition`1" /> condition
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // apply the condition to the collected tasks
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


