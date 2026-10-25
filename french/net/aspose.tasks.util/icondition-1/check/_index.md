---
title: "ICondition1.Check"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ICondition. Retourne true si l'objet spécifié satisfait les conditions"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Renvoie true si l'objet spécifié satisfait les conditions.

```csharp
public bool Check(T el)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | L'objet à vérifier. |

### Valeur de retour

Vrai si l'objet satisfait les conditions.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


