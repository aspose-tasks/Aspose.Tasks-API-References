---
title: "ListUtils.Find"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ListUtils. Trouver la première occurrence d'un élément de liste qui satisfait la condition spécifiée"
type: docs
weight: 30
url: /fr/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Trouver la première occurrence d'un élément de liste qui satisfait la condition spécifiée.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet à trouver. |
| liste | Une liste à traiter. |
| cond | Condition utilisée pour trouver un élément dans la liste spécifiée. |

### Valeur de retour

Élément de liste ou null.

## Exemples

Montre comment travailler avec la méthode Find de l'utilitaire de liste.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Retourne vrai si l'objet spécifié satisfait les conditions.
    /// </summary>
    /// <param name=\"el\">L'objet à vérifier.</param>
    /// <returns>Vrai si l'objet satisfait les conditions.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Voir aussi

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


