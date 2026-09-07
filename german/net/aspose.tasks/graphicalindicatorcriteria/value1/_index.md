---
title: "GraphicalIndicatorCriteria.Value1"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "GraphicalIndicatorCriteria-Eigenschaft. Gibt den Wert zurück, der zum Testen des Werts erweiterter Attribute verwendet wird."
type: docs
weight: 50
url: /de/net/aspose.tasks/graphicalindicatorcriteria/value1/
---
## GraphicalIndicatorCriteria.Value1 property

Ruft den Wert ab, der zum Testen des Wertes des erweiterten Attributs verwendet wird.

```csharp
public GraphicalIndicatorCriteriaValue Value1 { get; }
```

## Beispiele

Zeigt, wie man Informationen zu grafischen Indikatoren abruft.

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

### Siehe auch

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


