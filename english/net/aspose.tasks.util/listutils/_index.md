---
title: Class ListUtils
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.ListUtils class. Utility class for list processing
type: docs
weight: 2660
url: /net/aspose.tasks.util/listutils/
---
## ListUtils class

Utility class for list processing.

```csharp
public static class ListUtils
```

## Methods

| Name | Description |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Apply algorithm for each list element starting from specified position. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filter list elements by specified condition. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Find first occurrence of an list element which satisfy specified condition. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


