---
title: ListUtils.Apply
second_title: Aspose.Tasks for .NET API Reference
description: ListUtils method. Apply algorithm for each list element starting from specified position
type: docs
weight: 10
url: /net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Apply algorithm for each list element starting from specified position.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply algorithm to. |
| list | List to process. |
| algorithm | Applied algorithm. |
| startIndex | Start element position. |

## Examples

Shows how to work with list util Apply method.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### See Also

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


