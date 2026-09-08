---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GraphicalIndicatorCriteria. Obtiene el valor del enumerado GraphicalIndicatorCriteriaType que indica para qué filas se aplica el indicador"
type: docs
weight: 30
url: /es/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Obtiene el valor del enumerado [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) que indica para qué filas se aplica el indicador.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
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

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


