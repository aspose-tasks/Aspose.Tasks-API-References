---
title: "ListUtils.Filter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ListUtils. Filtrar elementos de la lista según la condición especificada"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filtrar elementos de la lista según la condición especificada.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar el filtro. |
| lista | Una lista para procesar. |
| cond | Condición utilizada para filtrar la lista especificada. |

### Valor devuelto

Lista filtrada.

## Ejemplos

Muestra cómo trabajar con el método Filter de la utilidad de listas.

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
    /// Devuelve verdadero si el objeto especificado cumple las condiciones.
    /// </summary>
    /// <param name=\"el\">El objeto a verificar.</param>
    /// <returns>Verdadero si el objeto cumple las condiciones.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Ver también

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


