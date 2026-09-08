---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GraphicalIndicatorCriteria eigenschap. Haalt het type vergelijking op dat wordt gemaakt tussen de waarde van uitgebreide attributen en waarden die dienen als criterium voor de toepassing van de grafische indicator. FilterComparisonType"
type: docs
weight: 40
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Haalt het type vergelijking op dat wordt gemaakt tussen de waarde van een uitgebreid attribuut en waarden die dienen als criterium voor de toepassing van de grafische indicator. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


