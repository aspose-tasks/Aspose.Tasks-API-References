---
title: "ExtendedAttribute.NumericValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute प्रॉपर्टी। संख्यात्मक प्रकार Cost Number वाले एट्रिब्यूट्स के लिए मान प्राप्त करता है या सेट करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/extendedattribute/numericvalue/
---
## ExtendedAttribute.NumericValue property

संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान प्राप्त करता है या सेट करता है।

```csharp
public decimal NumericValue { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि [`AttributeDefinition`](../attributedefinition/) प्रॉपर्टी प्रारंभ नहीं की गई है या [`AttributeDefinition`](../attributedefinition/) प्रॉपर्टी का कस्टम फ़ील्ड प्रकार 'Cost' या 'Number' नहीं है तो थ्रो किया जाता है। |

## उदाहरण

दिखाता है कि उपयोगकर्ता द्वारा निर्दिष्ट फ़ॉर्मूला का उपयोग करके मान की गणना किया गया कस्टम फ़ील्ड कैसे जोड़ा जाए।

```csharp
var project = new Project();

// नया टास्क विस्तारित गुण परिभाषा बनाएं
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// गुण में एक फ़ॉर्मूला जोड़ें।
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// विस्तारित एट्रिब्यूट बनाएं
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// हमने विस्तारित गुण के लिए फ़ॉर्मूला सेट किया, इसलिए यह केवल-पढ़ने योग्य है (मान फ़ॉर्मूला का उपयोग करके गणना किया जाता है)।
// आउटपुट है "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// आप केवल-पढ़ने योग्य फ़ील्ड का मान सेट करने का प्रयास कर सकते हैं, लेकिन इसका कोई प्रभाव नहीं पड़ेगा।
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### संबंधित देखें

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


