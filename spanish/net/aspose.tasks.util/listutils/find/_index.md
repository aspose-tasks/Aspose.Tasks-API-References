---
title: "ListUtils.Find"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ListUtils. Encontrar la primera ocurrencia de un elemento de la lista que cumpla la condición especificada"
type: docs
weight: 30
url: /es/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Encontrar la primera aparición de un elemento de la lista que cumpla la condición especificada.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto a buscar. |
| lista | Una lista para procesar. |
| cond | Condición utilizada para encontrar un elemento en la lista especificada. |

### Valor devuelto

Elemento de la lista o null.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


