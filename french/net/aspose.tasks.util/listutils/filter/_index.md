---
title: "ListUtils.Filter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ListUtils. Filtrer les éléments de la liste selon la condition spécifiée"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filtrer les éléments de la liste selon la condition spécifiée.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer le filtre. |
| liste | Une liste à traiter. |
| cond | Condition utilisée pour filtrer la liste spécifiée. |

### Valeur de retour

Liste filtrée.

## Exemples

Montre comment travailler avec la méthode Filter de list util.

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
    /// Retourne vrai si l'objet spécifié satisfait les conditions.
    /// </summary>
    /// <param name=\"el\">L'objet à vérifier.</param>
    /// <returns>Vrai si l'objet satisfait les conditions.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Voir aussi

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


