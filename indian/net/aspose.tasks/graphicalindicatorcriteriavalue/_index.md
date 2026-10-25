---
title: "क्लास GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaValue क्लास। ग्राफिकल संकेतक मानदंड की शर्त जाँच में उपयोग किए जाने वाले मान का प्रतिनिधित्व करता है।"
type: docs
weight: 750
url: /hi/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

ग्राफ़िकल इंडिकेटर मानदंड की शर्त जांच में उपयोग किए जाने वाले मान का प्रतिनिधित्व करता है।

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | स्थिर फ़्लैग (bool) मान के साथ GraphicalIndicatorCriteriaValue क्लास का एक उदाहरण बनाता है। |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | स्थिर DateTime मान के साथ GraphicalIndicatorCriteriaValue क्लास का एक उदाहरण बनाता है। |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | स्थिर दशमलव मान के साथ GraphicalIndicatorCriteriaValue क्लास का एक उदाहरण बनाता है। |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | स्थिर Duration मान के साथ GraphicalIndicatorCriteriaValue क्लास का एक उदाहरण बनाता है। |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | स्थिर स्ट्रिंग मान के साथ GraphicalIndicatorCriteriaValue क्लास का एक उदाहरण बनाता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | वर्तमान उदाहरण फ़ील्ड लिंक है या नहीं, यह प्राप्त करता है (फ़ील्ड के मान का प्रतिनिधित्व करता है)। |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | फ़ील्ड मान का अंतर्निहित स्थिरांक प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | निर्दिष्ट MS Project के फ़ील्ड का मान दर्शाने वाली GraphicalIndicatorCriteriaValue क्लास की एक इंस्टेंस बनाता है। |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |

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


