---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GraphicalIndicatorCriteria özelliği. IsWithin ve IsNotWithin karşılaştırma türlerinde genişletilmiş öznitelik değerini test etmek için kullanılan ikinci değeri alır."
type: docs
weight: 60
url: /tr/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

‘IsWithin’ ve ‘IsNotWithin’ karşılaştırma türleri durumunda genişletilmiş özniteliğin değerini test etmek için kullanılan ikinci değeri alır.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


