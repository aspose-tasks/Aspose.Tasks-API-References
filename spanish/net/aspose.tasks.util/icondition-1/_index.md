---
title: "Interfaz IConditionT"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Interfaz Aspose.Tasks.Util.ICondition1T. Representa una condición que puede ser usada por filtros o métodos de búsqueda"
type: docs
weight: 2720
url: /es/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Representa una condición que puede ser utilizada por filtros o métodos de búsqueda.

```csharp
public interface ICondition<in T>
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar la interfaz del método. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Devuelve true si el objeto especificado satisface las condiciones. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


