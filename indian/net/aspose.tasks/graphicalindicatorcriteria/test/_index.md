---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GraphicalIndicatorCriteria प्रॉपर्टी। विस्तारित एट्रिब्यूट्स वैल्यू और वैल्यूज़ के बीच की तुलना का प्रकार प्राप्त करता है जो ग्राफिकल इंडिकेटर के अनुप्रयोग के लिए मानदंड के रूप में कार्य करता है। FilterComparisonType"
type: docs
weight: 40
url: /hi/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

प्राप्त करता है विस्तारित एट्रिब्यूट के मान और वैल्यूज़ के बीच की तुलना का प्रकार जो ग्राफिकल इंडिकेटर के अनुप्रयोग के लिए मानदंड के रूप में कार्य करता है। [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


