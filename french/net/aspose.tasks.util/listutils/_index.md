---
title: "Classe ListUtils"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Util.ListUtils. Classe utilitaire pour le traitement des listes"
type: docs
weight: 2740
url: /fr/net/aspose.tasks.util/listutils/
---
## ListUtils class

Classe utilitaire pour le traitement des listes.

```csharp
public static class ListUtils
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filtrer les éléments de la liste selon la condition spécifiée. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Trouver la première occurrence d'un élément de liste qui satisfait la condition spécifiée. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


