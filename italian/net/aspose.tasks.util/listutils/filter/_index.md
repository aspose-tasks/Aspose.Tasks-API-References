---
title: "ListUtils.Filter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ListUtils. Filtra gli elementi della lista secondo la condizione specificata"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filtra gli elementi della lista secondo la condizione specificata.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare il filtro. |
| elenco | Una lista da elaborare. |
| cond | Condizione utilizzata per filtrare la lista specificata. |

### Valore di ritorno

Lista filtrata.

## Esempi

Mostra come utilizzare il metodo Filter di list util.

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
    /// Restituisce true se l'oggetto specificato soddisfa le condizioni.
    /// </summary>
    /// <param name=\"el\">L'oggetto da verificare.</param>
    /// <returns>True se l'oggetto soddisfa le condizioni.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Vedi anche

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


