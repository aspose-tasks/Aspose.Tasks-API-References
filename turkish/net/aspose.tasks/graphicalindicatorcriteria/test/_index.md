---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GraphicalIndicatorCriteria özelliği. Genişletilmiş öznitelik değeri ile değerler arasındaki karşılaştırma tipini alır; bu, grafik göstergenin uygulanması için bir kriter olarak işlev görür. FilterComparisonType"
type: docs
weight: 40
url: /tr/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

Genişletilmiş öznitelik değerinin ve değerlerin arasındaki karşılaştırma tipini alır; bu, grafik göstergenin uygulanması için bir kriter olarak işlev görür. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
```

## Örnekler

Grafik göstergeleri bilgilerini nasıl alacağınızı gösterir.

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

### Ayrıca Bakınız

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


