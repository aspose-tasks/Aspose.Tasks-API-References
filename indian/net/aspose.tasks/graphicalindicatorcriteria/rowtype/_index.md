---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GraphicalIndicatorCriteria प्रॉपर्टी। GraphicalIndicatorCriteriaType एनीम का मान प्राप्त करता है जो दर्शाता है कि संकेतक किन पंक्तियों पर लागू होता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

प्राप्त करता है [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) एनीम का मान जो दर्शाता है कि संकेतक किन पंक्तियों पर लागू होता है।

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## उदाहरण

ग्राफ़िकल इंडिकेटर्स की जानकारी कैसे प्राप्त करें, यह दर्शाता है।

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

### संबंधित देखें

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


