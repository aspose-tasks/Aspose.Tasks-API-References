---
title: "Interfaccia IConditionT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.Util.ICondition1T. Rappresenta una condizione che può essere utilizzata da filtri o metodi di ricerca"
type: docs
weight: 2720
url: /it/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Rappresenta una condizione che può essere usata da filtri o metodi di ricerca.

```csharp
public interface ICondition<in T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Restituisce true se l'oggetto specificato soddisfa le condizioni. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


