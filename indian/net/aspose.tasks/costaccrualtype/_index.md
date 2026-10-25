---
title: "एनम CostAccrualType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CostAccrualType एनम। एक संचित लागत के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 350
url: /hi/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

अक्रूअल लागत के प्रकार को निर्दिष्ट करता है।

```csharp
public enum CostAccrualType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | संकेत करता है कि अपरिभाषित मान का अर्थ है कि फ़ील्ड मूल परियोजना फ़ाइल में परिभाषित नहीं था। |
| Start | `0` | प्रारंभ लागत संचित प्रकार को दर्शाता है। |
| Prorated | `1` | प्रोरेटेड लागत संचित प्रकार को दर्शाता है। |
| End | `2` | समाप्ति लागत संचित प्रकार को दर्शाता है। |
| Invalid | `3` | अमान्य लागत संचित प्रकार को दर्शाता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि संसाधन मानक और ओवरटाइम लागतें कब और कैसे चार्ज की जाएँगी, या संचित की जाएँगी (संचित विधि: निर्धारित करती है कि किसी संसाधन की लागत कब उत्पन्न होती है और वास्तविक लागतें कब परियोजना में चार्ज की जाती हैं। आप लागत को कार्य की शुरुआत [Start] या समाप्ति [End] पर ले सकते हैं या कार्य के दौरान उन्हें [Prorated] कर सकते हैं), कार्य की लागत (CostAccrualType.End) तक।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// लागत संचित प्रकार सेट करें
// यदि आप समाप्ति विकल्प चुनते हैं, तो लागतें तब तक संचित नहीं होतीं जब तक शेष कार्य शून्य न हो जाए।
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// परियोजना के साथ काम करें...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


