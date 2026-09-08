---
title: "Interfaz IAlgorithmT"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Interfaz Aspose.Tasks.Util.IAlgorithm1T. Representa un algoritmo que puede aplicarse a una lista de objetos T"
type: docs
weight: 2710
url: /es/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Representa un algoritmo que puede aplicarse a una lista de objetos *T*.

```csharp
public interface IAlgorithm<in T>
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar la interfaz del método. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Procesa un objeto en la lista. Llamado después de [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Llamado después del procesamiento de un objeto. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Llamado antes del procesamiento de un objeto. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


