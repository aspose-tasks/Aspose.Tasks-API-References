---
title: "ICondition1.Check"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ICondition. Devuelve true si el objeto especificado cumple las condiciones"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Devuelve true si el objeto especificado satisface las condiciones.

```csharp
public bool Check(T el)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | El objeto a comprobar. |

### Valor devuelto

Verdadero si el objeto cumple las condiciones.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


