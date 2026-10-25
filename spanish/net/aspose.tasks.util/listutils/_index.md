---
title: "Clase ListUtils"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.ListUtils. Clase de utilidad para el procesamiento de listas"
type: docs
weight: 2740
url: /es/net/aspose.tasks.util/listutils/
---
## ListUtils class

Clase de utilidad para el procesamiento de listas.

```csharp
public static class ListUtils
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Aplicar algoritmo para cada elemento de la lista a partir de la posición especificada. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filtrar elementos de la lista según la condición especificada. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Encontrar la primera aparición de un elemento de la lista que cumpla la condición especificada. |

## Ejemplos

Muestra cómo trabajar con el método Find de la utilidad de listas.

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
    /// Devuelve verdadero si el objeto especificado cumple las condiciones.
    /// </summary>
    /// <param name=\"el\">El objeto a verificar.</param>
    /// <returns>Verdadero si el objeto cumple las condiciones.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Ver también

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


