---
title: "Enum RollupType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RollupType enum. रोलअप प्रकार को निर्दिष्ट करता है"
type: docs
weight: 1950
url: /hi/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

रोलअप प्रकार को निर्दिष्ट करता है।

```csharp
public enum RollupType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Null | `0` | नल रोलअप प्रकार को दर्शाता है। |
| Maximum | `1` | अधिकतम रोलअप प्रकार को दर्शाता है। |
| Minimum | `2` | न्यूनतम रोलअप प्रकार को दर्शाता है। |
| Count | `3` | गणना रोलअप प्रकार को दर्शाता है। |
| Sum | `4` | योग रोलअप प्रकार को दर्शाता है। |
| Average | `5` | औसत रोलअप प्रकार को दर्शाता है। |
| AverageFirstSublevel | `6` | औसत प्रथम उपस्तर रोलअप प्रकार को दर्शाता है। |
| CountFirstSublevel | `7` | गणना प्रथम उपस्तर रोलअप प्रकार को दर्शाता है। |
| CountNonsummaries | `8` | गणना गैर-सारांश रोलअप प्रकार को दर्शाता है। |

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


