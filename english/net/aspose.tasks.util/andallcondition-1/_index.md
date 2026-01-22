---
title: Class AndAllConditionT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.AndAllCondition1T class. Applies logical AND to all conditions. For example cond1 AND cond2 AND cond3
type: docs
weight: 2630
url: /net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Applies logical AND to all conditions. For example: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply method interface to. |

## Constructors

| Name | Description |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Initializes a new instance of the `AndAllCondition` class. |

## Methods

| Name | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Returns true if the specified object satisfy the conditions. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


