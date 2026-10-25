---
title: "Interface IConditionT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.ICondition1T interface. Vertegenwoordigt een voorwaarde die kan worden gebruikt door filters of zoekmethoden"
type: docs
weight: 2720
url: /nl/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Stelt een voorwaarde voor die kan worden gebruikt door filters of zoekmethoden.

```csharp
public interface ICondition<in T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


