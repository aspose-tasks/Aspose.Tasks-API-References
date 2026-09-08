---
title: "ICondition1.Check"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ICondition-methode. Retourneert true als het opgegeven object aan de voorwaarden voldoet"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Retourneert true als het opgegeven object aan de voorwaarden voldoet.

```csharp
public bool Check(T el)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

### Retourwaarde

True als het object aan de voorwaarden voldoet.

## Voorbeelden

Toont hoe te werken met de lijstutil Filter-methode.

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
    /// Retourneert true als het opgegeven object aan de voorwaarden voldoet.
    /// </summary>
    /// <param name=\"el\">Het object om te controleren.</param>
    /// <returns>True als het object aan de voorwaarden voldoet.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Zie ook

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


