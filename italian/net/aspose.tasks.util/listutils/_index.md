---
title: "Classe ListUtils"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.ListUtils. Classe di utilità per l'elaborazione delle liste"
type: docs
weight: 2740
url: /it/net/aspose.tasks.util/listutils/
---
## ListUtils class

Classe di utilità per l'elaborazione delle liste.

```csharp
public static class ListUtils
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Applica l'algoritmo a ogni elemento della lista a partire dalla posizione specificata. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filtra gli elementi della lista secondo la condizione specificata. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Trova la prima occorrenza di un elemento della lista che soddisfa la condizione specificata. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


