---
title: "GraphicalIndicatorCriteria.Value1"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GraphicalIndicatorCriteria eigenschap. Haalt de waarde op die wordt gebruikt om de waarde van uitgebreide attributen te testen"
type: docs
weight: 50
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/value1/
---
## GraphicalIndicatorCriteria.Value1 property

Haalt de waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen.

```csharp
public GraphicalIndicatorCriteriaValue Value1 { get; }
```

## Voorbeelden

Toont hoe grafische indicatorinformatie op te halen.

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

### Zie ook

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


