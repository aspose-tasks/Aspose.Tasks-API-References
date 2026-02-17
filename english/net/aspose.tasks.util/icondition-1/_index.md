---
title: Interface IConditionT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.ICondition1T interface. Represents a condition which can be used by filters or search methods
type: docs
weight: 2700
url: /net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Represents a condition which can be used by filters or search methods.

```csharp
public interface ICondition<in T>
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply method interface to. |

## Methods

| Name | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Returns true if the specified object satisfy the conditions. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


