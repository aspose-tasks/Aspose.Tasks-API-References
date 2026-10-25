---
title: "ExtendedAttributeDefinition.RollupType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। रोलअप्स की गणना करने के तरीके को प्राप्त करता है या सेट करता है।"
type: docs
weight: 230
url: /hi/net/aspose.tasks/extendedattributedefinition/rolluptype/
---
## ExtendedAttributeDefinition.RollupType property

रोलअप्स की गणना करने के तरीके को प्राप्त करता है या सेट करता है।

```csharp
public RollupType RollupType { get; set; }
```

## टिप्पणियाँ

वर्तमान में केवल Xml फ़ॉर्मेट के लिए लेखन समर्थित है।

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

* enum [RollupType](../../rolluptype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


