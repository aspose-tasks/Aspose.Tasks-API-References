---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GraphicalIndicatorCriteria. Obtiene el segundo valor utilizado para probar el valor de atributos extendidos en caso de los tipos de comparación IsWithin e IsNotWithin"
type: docs
weight: 60
url: /es/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Obtiene el segundo valor utilizado para probar el valor del atributo extendido en caso de los tipos de comparación 'IsWithin' y 'IsNotWithin'.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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


