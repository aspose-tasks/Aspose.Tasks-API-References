---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GraphicalIndicatorCriteria eigenschap. Haalt de waarde op van de GraphicalIndicatorCriteriaType enum die aangeeft voor welke rijen de indicator wordt toegepast"
type: docs
weight: 30
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

Haalt de waarde op van de [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum die aangeeft voor welke rijen de indicator wordt toegepast.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
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

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


