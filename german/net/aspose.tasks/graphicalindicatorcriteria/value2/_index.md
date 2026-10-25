---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "GraphicalIndicatorCriteria-Eigenschaft. Gibt den zweiten Wert zurück, der verwendet wird, um den Wert erweiterter Attribute bei den Vergleichstypen IsWithin und IsNotWithin zu testen"
type: docs
weight: 60
url: /de/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Ruft den zweiten Wert ab, der zum Testen des Wertes des erweiterten Attributs im Fall der Vergleichstypen 'IsWithin' und 'IsNotWithin' verwendet wird.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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


