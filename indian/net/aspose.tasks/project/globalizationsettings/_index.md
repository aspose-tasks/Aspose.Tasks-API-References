---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। प्रोजेक्ट की ग्लोबलाइज़ेशन भाषा-विशिष्ट सेटिंग्स प्राप्त करता है या सेट करता है"
type: docs
weight: 460
url: /hi/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

परियोजना की ग्लोबलाइज़ेशन (भाषा-विशिष्ट) सेटिंग्स प्राप्त करता है या सेट करता है।

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## टिप्पणियाँ

सिफ़ारिश किया गया तरीका है कि पूरे प्रोजेक्ट में संस्कृति-निर्भर नहीं वाले लिटरल या फ़ॉर्मेट का उपयोग किया जाए। हालांकि, यदि कोई प्रोजेक्ट संस्कृति-विशिष्ट लिटरल का उपयोग करता है, तो यह क्लास गणना इंजन को उन लिटरलों को पार्स करने में मदद करने के लिए उपयोग की जा सकती है।

## उदाहरण

प्रोजेक्ट की भाषा-विशिष्ट सेटिंग्स को कैसे सेट किया जाए, यह दिखाता है।

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// विस्तारित एट्रिब्यूट बनाएं
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### संबंधित देखें

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


