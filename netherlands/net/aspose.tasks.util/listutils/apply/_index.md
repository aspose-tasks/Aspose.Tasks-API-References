---
title: "ListUtils.Apply"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ListUtils-methode. Pas algoritme toe op elk lijstonderdeel beginnend vanaf de opgegeven positie"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Pas het algoritme toe op elk lijstelement beginnend vanaf de opgegeven positie.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop het algoritme moet worden toegepast. |
| lijst | Lijst om te verwerken. |
| algoritme | Toegepast algoritme. |
| startIndex | Startpositie van het element. |

## Voorbeelden

Toont hoe te werken met de lijst util Apply-methode.

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

### Zie ook

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


