---
title: "GraphicalIndicatorCriteria.Value1"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GraphicalIndicatorCriteria. Obtiene el valor usado para probar el valor de los atributos extendidos"
type: docs
weight: 50
url: /es/net/aspose.tasks/graphicalindicatorcriteria/value1/
---
## GraphicalIndicatorCriteria.Value1 property

Obtiene el valor utilizado para probar el valor del atributo extendido.

```csharp
public GraphicalIndicatorCriteriaValue Value1 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


