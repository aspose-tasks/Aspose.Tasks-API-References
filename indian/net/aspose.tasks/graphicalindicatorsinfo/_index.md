---
title: "Class GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GraphicalIndicatorsInfo क्लास। विस्तारित एट्रिब्यूट से जुड़ी ग्राफिकल इंडिकेटर्स परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 760
url: /hi/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

एक विस्तारित विशेषता से जुड़ी ग्राफ़िकल इंडिकेटर परिभाषा का प्रतिनिधित्व करता है।

```csharp
public sealed class GraphicalIndicatorsInfo
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | `GraphicalIndicatorsInfo` प्रकार का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | ग्राफ़िकल संकेत मानदंडों की सूची प्राप्त करता है। |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | प्रोजेक्ट सारांश पंक्ति को सारांश पंक्तियों से मानदंड विरासत में मिलते हैं या नहीं, यह दर्शाने वाला फ़्लैग प्राप्त करता है या सेट करता है। |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | फ़ील्ड के डेटा मानों को टूलटिप्स में दिखाया जाना चाहिए या नहीं, यह दर्शाने वाला फ़्लैग प्राप्त करता है या सेट करता है। |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | सारांश पंक्तियों को गैर‑सारांश पंक्तियों से मानदंड विरासत में मिलते हैं या नहीं, यह दर्शाने वाला फ़्लैग प्राप्त करता है या सेट करता है। |

## उदाहरण

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


