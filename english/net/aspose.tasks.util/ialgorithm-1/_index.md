---
title: Interface IAlgorithmT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.IAlgorithm1T interface. Represents an algorithm that can be applied to a list of objects T
type: docs
weight: 2630
url: /net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Represents an algorithm that can be applied to a list of objects *T*.

```csharp
public interface IAlgorithm<in T>
```

| Parameter | Description |
| --- | --- |
| T | The type of object to apply method interface to. |

## Methods

| Name | Description |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Processes an object in the list. Called after [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Called after processing of an object. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Called before processing of an object. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


