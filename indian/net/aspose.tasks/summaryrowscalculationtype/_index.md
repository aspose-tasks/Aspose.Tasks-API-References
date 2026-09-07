---
title: "Enum SummaryRowsCalculationType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.SummaryRowsCalculationType enum. सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट मान की गणना प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 2310
url: /hi/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट मान की गणना के प्रकार को निर्दिष्ट करता है।

```csharp
public enum SummaryRowsCalculationType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | अर्थ है कि सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट का मान गणना नहीं किया जाता। |
| Rollup | `1` | अर्थ है कि सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट का मान [`RollupType`](../extendedattributedefinition/rolluptype/) में परिभाषित रोलअप फ़ंक्शन का उपयोग करके गणना किया जाता है। |
| UseFormula | `2` | अर्थ है कि सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट का मान [`Formula`](../extendedattributedefinition/formula/) में परिभाषित सूत्र का उपयोग करके गणना किया जाता है। |

## उदाहरण

विस्तारित गुण परिभाषा के गणना प्रकार के साथ कैसे काम करें, यह दर्शाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// लीफ़ टास्क और सारांश टास्क के मानों की गणना फ़ॉर्मूला द्वारा की जाने वाली 'Formula' प्रकार के साथ गुण परिभाषा बनाएं।
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// सारांश टास्क के मानों की गणना 'Average' रोलअप प्रकार द्वारा की जाने वाली गुण परिभाषा बनाएं।
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


