---
title: "ListUtils.Find"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ListUtils. Trova la prima occorrenza di un elemento della lista che soddisfa la condizione specificata"
type: docs
weight: 30
url: /it/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Trova la prima occorrenza di un elemento della lista che soddisfa la condizione specificata.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto da trovare. |
| elenco | Una lista da elaborare. |
| cond | Condizione utilizzata per trovare un elemento nella lista specificata. |

### Valore di ritorno

Elemento della lista o null.

## Esempi

Mostra come lavorare con il metodo Find dell'utilità di lista.

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
    /// Restituisce true se l'oggetto specificato soddisfa le condizioni.
    /// </summary>
    /// <param name=\"el\">L'oggetto da verificare.</param>
    /// <returns>True se l'oggetto soddisfa le condizioni.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Vedi anche

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


