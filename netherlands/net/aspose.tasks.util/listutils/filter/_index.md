---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ListUtils-methode. Filter lijstonderdelen op opgegeven voorwaarde"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filter lijstelementen op basis van de opgegeven voorwaarde.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop het filter moet worden toegepast. |
| lijst | Een lijst om te verwerken. |
| cond | Voorwaarde die wordt gebruikt om de opgegeven lijst te filteren. |

### Retourwaarde

Gefilterde lijst.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


