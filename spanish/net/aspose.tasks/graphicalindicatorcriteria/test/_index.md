---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GraphicalIndicatorCriteria. Obtiene el tipo de comparación realizado entre el valor de los atributos extendidos y los Valores que actúan como criterio para la aplicación del indicador gráfico. FilterComparisonType"
type: docs
weight: 40
url: /es/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Obtiene el tipo de comparación realizado entre el valor del atributo extendido y los Valores que actúan como criterio para la aplicación del indicador gráfico. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
```

## Ejemplos

Muestra cómo recuperar la información de indicadores gráficos.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

### Ver también

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


