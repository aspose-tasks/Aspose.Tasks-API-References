---
title: "एनम GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType एनम। ग्राफिकल इंडिकेटर मानदंड की प्लेसमेंट दर्शाता है।"
type: docs
weight: 740
url: /hi/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

ग्राफ़िकल संकेतक मानदंडों की स्थिति को दर्शाता है।

```csharp
public enum GraphicalIndicatorCriteriaType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| NonSummaryRows | `0` | गैर-सारांश पंक्तियों को दर्शाता है। |
| SummaryRows | `1` | सारांश पंक्तियों को दर्शाता है। |
| ProjectSummary | `2` | प्रोजेक्ट सारांश टास्क पंक्ति को दर्शाता है। |

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


