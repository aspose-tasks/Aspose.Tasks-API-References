---
title: "क्लास GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GraphicalIndicatorCriteria क्लास। विस्तारित एट्रिब्यूट से जुड़ी एक ग्राफिकल इंडिकेटर मानदंड का प्रतिनिधित्व करता है।"
type: docs
weight: 730
url: /hi/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

एक विस्तारित विशेषता से जुड़ी एक ग्राफ़िकल इंडिकेटर मानदंड का प्रतिनिधित्व करता है।

```csharp
public sealed class GraphicalIndicatorCriteria
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` प्रकार का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` प्रकार का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | फ़ील्ड मानदंडों को पूरा करने पर प्रदर्शित करने के लिए इमेज का इंडेक्स प्राप्त करता है। |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) एनीम का मान प्राप्त करता है जो दर्शाता है कि किन पंक्तियों पर इंडिकेटर लागू किया जाता है। |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | विस्तारित एट्रिब्यूट के मान और उन मानों के बीच किए गए तुलना प्रकार को प्राप्त करता है जो ग्राफिकल इंडिकेटर के अनुप्रयोग के लिए मानदंड के रूप में कार्य करते हैं। [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | विस्तारित विशेषता के मान का परीक्षण करने के लिए उपयोग किया जाने वाला मान प्राप्त करता है। |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | 'IsWithin' और 'IsNotWithin' तुलना प्रकारों के मामले में विस्तारित विशेषता के मान का परीक्षण करने के लिए उपयोग किया जाने वाला दूसरा मान प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | `GraphicalIndicatorCriteria` क्लास की इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है। |

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

विस्तारित विशेषता के लिए ग्राफ़िकल इंडिकेटर कैसे सेट करें, यह दर्शाता है।

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// 'IsWithin' मानदंड को 2 मानों की आवश्यकता होती है।
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue' मानदंड को मानों की आवश्यकता नहीं होती।
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


