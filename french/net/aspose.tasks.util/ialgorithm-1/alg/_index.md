---
title: "IAlgorithm1.Alg"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode IAlgorithm. Traite un objet dans la liste. Appelée après PreAlg"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/ialgorithm-1/alg/
---
## IAlgorithm&lt;T&gt;.Alg method

Traite un objet dans la liste. Appelée après [`PreAlg`](../prealg/);

```csharp
public void Alg(T el, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Objet traité. |
| index | Int32 | Index de l'objet. |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)


