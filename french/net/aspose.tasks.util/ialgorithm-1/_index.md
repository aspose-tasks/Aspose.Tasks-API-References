---
title: "Interface IAlgorithmT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.IAlgorithm1T interface. Représente un algorithme qui peut être appliqué à une liste d'objets T"
type: docs
weight: 2710
url: /fr/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Représente un algorithme qui peut être appliqué à une liste d'objets *T*.

```csharp
public interface IAlgorithm<in T>
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'interface de méthode. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Traite un objet dans la liste. Appelé après [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Appelé après le traitement d'un objet. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Appelé avant le traitement d'un objet. |

## Exemples

Montre comment travailler avec la méthode Apply de list util.

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

### Voir aussi

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


