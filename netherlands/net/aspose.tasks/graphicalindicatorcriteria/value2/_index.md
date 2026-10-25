---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GraphicalIndicatorCriteria-eigenschap. Haalt de tweede waarde op die wordt gebruikt om de waarde van uitgebreide attributen te testen in het geval van IsWithin- en IsNotWithin-vergelijkingstypen."
type: docs
weight: 60
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

Haalt de tweede waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen in het geval van de vergelijkingssoorten 'IsWithin' en 'IsNotWithin'.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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


