---
title: "Interface IAlgorithmT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.IAlgorithm1T interface. Vertegenwoordigt een algoritme dat kan worden toegepast op een lijst van objecten T"
type: docs
weight: 2710
url: /nl/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Stelt een algoritme voor dat kan worden toegepast op een lijst van objecten *T*.

```csharp
public interface IAlgorithm<in T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Verwerkt een object in de lijst. Aangeroepen na [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Aangeroepen na verwerking van een object. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Aangeroepen vóór verwerking van een object. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


