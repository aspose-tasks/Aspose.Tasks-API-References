---
title: ListUtils.Find
second_title: Aspose.Tasks for .NET API Reference
description: ListUtils method. Find first occurrence of an list element which satisfy specified condition
type: docs
weight: 30
url: /net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Find first occurrence of an list element which satisfy specified condition.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Description |
| --- | --- |
| T | The type of object to find. |
| list | A list to process. |
| cond | Condition used to find an element in the specified list. |

### Return Value

List element or null.

## Examples

Shows how to work with list util Find method.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Returns true if the specified object satisfy the conditions.
    /// </summary>
    /// <param name="el">The object to check.</param>
    /// <returns>True if the object satisfy the conditions.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### See Also

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


