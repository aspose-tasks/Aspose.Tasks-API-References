---
title: "एनम CalculationType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalculationType enum. कस्टम एट्रिब्यूट्स मान की गणना के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 220
url: /hi/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

कस्टम एट्रिब्यूट मान की गणना के प्रकार को निर्दिष्ट करता है।

```csharp
public enum CalculationType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | इसका अर्थ है कि विस्तारित एट्रिब्यूट के पास कोई फ़ॉर्मूला लुकअप टेबल नहीं है और यह केवल उपयोगकर्ता द्वारा सेट किया गया मान संग्रहीत करता है। |
| Lookup | `1` | इसका अर्थ है कि विस्तारित एट्रिब्यूट का मान लुकअप टेबल के मानों तक सीमित है। |
| Formula | `2` | इसका अर्थ है कि विस्तारित एट्रिब्यूट का मान [`Formula`](../extendedattributedefinition/formula/) में परिभाषित फ़ॉर्मूला का उपयोग करके गणना किया जाता है। |

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


