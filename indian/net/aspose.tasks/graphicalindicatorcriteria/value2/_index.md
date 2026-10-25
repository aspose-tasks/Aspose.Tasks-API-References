---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GraphicalIndicatorCriteria प्रॉपर्टी। IsWithin और IsNotWithin तुलना प्रकारों के मामले में विस्तारित एट्रिब्यूट्स वैल्यू का परीक्षण करने के लिए उपयोग किया जाने वाला दूसरा मान प्राप्त करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

'IsWithin' और 'IsNotWithin' तुलना प्रकारों के मामले में विस्तारित विशेषता के मान का परीक्षण करने के लिए उपयोग किया जाने वाला दूसरा मान प्राप्त करता है।

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


