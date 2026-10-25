---
title: "Class GlobalizationSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GlobalizationSettings class. प्रोजेक्ट की ग्लोबलाइज़ेशन सेटिंग्स का प्रतिनिधित्व करता है।"
type: docs
weight: 720
url: /hi/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

प्रोजेक्ट की ग्लोबलाइज़ेशन सेटिंग्स का प्रतिनिधित्व करता है।

```csharp
public class GlobalizationSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | फ़ॉर्मूला में उपयोग किए गए बूलियन 'false' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है। |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | डेट फ़ील्ड के फ़ॉर्मूला में उपयोग किए गए "NA" (खाली मान) लिटरल को प्राप्त करता है। |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | फ़ॉर्मूले में उपयोग किए गए बूलियन 'true' लिटरल के लिए एक स्ट्रिंग प्राप्त करता है। |

## टिप्पणियाँ

परियोजना में संस्कृति-निर्भर नहीं लिटरल या फ़ॉर्मेट का उपयोग करने की अनुशंसित विधि है। हालांकि, यदि कोई परियोजना संस्कृति-विशिष्ट लिटरल का उपयोग करती है, तो इस क्लास का उपयोग फ़ॉर्मूला-गणना इंजन को उन लिटरल को पार्स करने में मदद करने के लिए किया जा सकता है।

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


