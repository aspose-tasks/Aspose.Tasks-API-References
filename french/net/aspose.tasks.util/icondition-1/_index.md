---
title: "Interface IConditionT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.ICondition1T interface. Représente une condition qui peut être utilisée par les filtres ou les méthodes de recherche."
type: docs
weight: 2720
url: /fr/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Représente une condition qui peut être utilisée par des filtres ou des méthodes de recherche.

```csharp
public interface ICondition<in T>
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'interface de méthode. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Renvoie true si l'objet spécifié satisfait les conditions. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


