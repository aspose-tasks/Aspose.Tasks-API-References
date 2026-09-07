---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "GraphicalIndicatorCriteria-Eigenschaft. Gibt den Vergleichstyp zurück, der zwischen dem Wert erweiterter Attribute und den Werten durchgeführt wird und als Kriterium für die Anwendung des grafischen Indikators dient. FilterComparisonType"
type: docs
weight: 40
url: /de/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Gibt den Vergleichstyp zurück, der zwischen dem Wert eines erweiterten Attributs und den Werten durchgeführt wird und als Kriterium für die Anwendung des grafischen Indikators dient. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


