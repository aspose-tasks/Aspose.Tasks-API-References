---
title: "क्लास ExtendedAttribute"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ExtendedAttribute क्लास। विस्तारित गुणों का प्रतिनिधित्व करता है"
type: docs
weight: 520
url: /hi/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

विस्तारित गुणों का प्रतिनिधित्व करता है।

```csharp
public class ExtendedAttribute
```

## गुण

| नाम | विवरण |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | गुण परिभाषा प्राप्त करता है। |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | तारीख प्रकार (Date, Start, Finish) वाले गुणों के लिए मान प्राप्त करता है या सेट करता है। |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | 'Duration' प्रकार वाले गुणों के लिए मान प्राप्त करता है या सेट करता है। |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | फ़ील्ड की आईडी प्राप्त करता है। |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | 'Flag' प्रकार वाले गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | विस्तारित गुण के मान की गणना में त्रुटि हुई है या नहीं, यह प्राप्त करता है। |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान प्राप्त करता है या सेट करता है। |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | 'Text' प्रकार वाले गुणों के लिए मान प्राप्त करता है या सेट करता है। |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | लुकअप मान का GUID प्राप्त करता है। |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | इस `ExtendedAttribute` इंस्टेंस का मान केवल-पढ़ने योग्य है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। यदि इस ऑब्जेक्ट के लिए [`ExtendedAttributeDefinition`](../extendedattributedefinition/) में कोई फ़ॉर्मूला या रोलअप परिभाषित है तो true लौटाता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | विस्तारित गुण का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। |

## टिप्पणियाँ

वर्तमान में MSP Xml 2003/2007 और mpp 2003 से विस्तारित गुणों के सभी प्रकारों को पढ़ना समर्थित है। MSP mpp 2007 के लिए सभी विस्तारित गुणों का पढ़ना समर्थित है, सिवाय अवधि (durations) और फ़्लैग (flags) के।

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


