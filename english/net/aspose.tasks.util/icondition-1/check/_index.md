---
title: ICondition1.Check
second_title: Aspose.Tasks for .NET API Reference
description: ICondition method. Returns true if the specified object satisfy the conditions
type: docs
weight: 10
url: /net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


