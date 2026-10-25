---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute प्रॉपर्टी। Text प्रकार वाले एट्रिब्यूट्स के लिए मान प्राप्त करता है या सेट करता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

'Text' प्रकार वाले गुणों के लिए मान प्राप्त करता है या सेट करता है।

```csharp
public string TextValue { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि [`AttributeDefinition`](../attributedefinition/) प्रॉपर्टी प्रारंभ नहीं की गई है या वर्तमान एट्रिब्यूट टेक्स्ट एट्रिब्यूट नहीं है तो थ्रो किया जाता है। |

## उदाहरण

दिखाता है कि MS Project तिथि/समय फ़ॉर्मूले का उपयोग करने वाले विस्तारित एट्रिब्यूट्स को कैसे जोड़ें।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// ProjDateDiff फ़ॉर्मूला सेट करें और विस्तारित एट्रिब्यूट मान प्रिंट करें
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// ProjDateSub फ़ॉर्मूला सेट करें और विस्तारित एट्रिब्यूट मान प्रिंट करें
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// हम ProjDurConv फ़ॉर्मूला को duration-मान वाले एट्रिब्यूट और text-मान वाले एट्रिब्यूट दोनों पर सेट कर सकते हैं।
// ProjDurConv फ़ॉर्मूला को duration-मान वाले विस्तारित एट्रिब्यूट पर सेट करें और उसका मान प्रिंट करें।
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// ProjDurConv फ़ॉर्मूला को text-मान वाले विस्तारित एट्रिब्यूट पर सेट करें और उसका मान प्रिंट करें।
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Second फ़ॉर्मूला सेट करें और विस्तारित एट्रिब्यूट मान प्रिंट करें
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Weekday फ़ॉर्मूला सेट करें और विस्तारित एट्रिब्यूट मान प्रिंट करें
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### संबंधित देखें

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


