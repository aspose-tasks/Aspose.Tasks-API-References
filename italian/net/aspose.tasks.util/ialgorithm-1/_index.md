---
title: "Interfaccia IAlgorithmT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Util.IAlgorithm1T interfaccia. Rappresenta un algoritmo che può essere applicato a un elenco di oggetti T"
type: docs
weight: 2710
url: /it/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Rappresenta un algoritmo che può essere applicato a un elenco di oggetti *T*.

```csharp
public interface IAlgorithm<in T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Elabora un oggetto nell'elenco. Chiamato dopo [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Chiamato dopo l'elaborazione di un oggetto. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Chiamato prima dell'elaborazione di un oggetto. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


