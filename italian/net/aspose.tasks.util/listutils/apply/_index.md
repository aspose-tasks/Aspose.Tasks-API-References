---
title: "ListUtils.Apply"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ListUtils. Applica l'algoritmo a ciascun elemento della lista a partire dalla posizione specificata"
type: docs
weight: 10
url: /it/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Applica l'algoritmo a ogni elemento della lista a partire dalla posizione specificata.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'algoritmo. |
| elenco | Lista da elaborare. |
| algoritmo | Algoritmo applicato. |
| startIndex | Posizione dell'elemento iniziale. |

## Esempi

Mostra come lavorare con il metodo Apply della utilità di elenco.

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

### Vedi anche

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


