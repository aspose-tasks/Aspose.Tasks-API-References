---
title: "ListUtils.Apply"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ListUtils. Aplicar algoritmo a cada elemento de la lista comenzando desde la posición especificada"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Aplicar algoritmo para cada elemento de la lista a partir de la posición especificada.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar el algoritmo. |
| lista | Lista para procesar. |
| algoritmo | Algoritmo aplicado. |
| startIndex | Posición del elemento inicial. |

## Ejemplos

Muestra cómo trabajar con el método Apply de la utilidad de listas.

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

### Ver también

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


