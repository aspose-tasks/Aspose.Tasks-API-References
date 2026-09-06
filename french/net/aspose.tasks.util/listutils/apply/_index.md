---
title: "ListUtils.Apply"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ListUtils. Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'algorithme. |
| liste | Liste à traiter. |
| algorithme | Algorithme appliqué. |
| startIndex | Position de l'élément de départ. |

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

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


