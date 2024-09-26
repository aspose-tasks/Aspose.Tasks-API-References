---
title: ListUtils.Filter
second_title: Aspose.Tasks for .NET API Reference
description: ListUtils method. Filter list elements by specified condition
type: docs
weight: 20
url: /net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filter list elements by specified condition.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply filter to. |
| list | A list to process. |
| cond | Condition used to filter the specified list. |

### Return Value

Filtered list.

## Examples

Shows how to work with list util Filter method.

```csharp
public void WorkWithListUtilsFilter()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Filter(filters, new FilterByIndex(1));

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

public class FilterByIndex : ICondition<Filter>
{
    private readonly int index;

    public FilterByIndex(int index)
    {
        this.index = index;
    }

    /// <summary>
    /// Returns true if the specified object satisfy the conditions.
    /// </summary>
    /// <param name="el">The object to check.</param>
    /// <returns>True if the object satisfy the conditions.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### See Also

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


