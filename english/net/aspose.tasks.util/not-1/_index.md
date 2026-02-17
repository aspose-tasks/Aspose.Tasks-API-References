---
title: Class NotT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.Not1T class. Applies logical NOT to the specified condition
type: docs
weight: 2730
url: /net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Applies logical NOT to the specified condition.

```csharp
public class Not<T> : ICondition<T>
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply method interface to. |

## Constructors

| Name | Description |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Initializes a new instance of the `Not` class. |

## Methods

| Name | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Returns true if the specified object satisfy the condition. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


