---
title: "Enum EarnedValueMethodType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.EarnedValueMethodType enum. अर्जित मूल्य की गणना के लिए उपयोग की जाने वाली विधि को निर्दिष्ट करता है"
type: docs
weight: 480
url: /hi/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

कमाए गए मूल्य की गणना के लिए उपयोग की जाने वाली विधि को निर्दिष्ट करता है।

```csharp
public enum EarnedValueMethodType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | फ़ील्ड मूल प्रोजेक्ट फ़ाइल में परिभाषित नहीं था। |
| PercentComplete | `0` | प्रतिशत पूर्ण |
| PhysicalPercentComplete | `1` | भौतिक प्रतिशत पूर्ण |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि अर्जित मूल्य की गणना के लिए उपयोग की जाने वाली विधि (EarnedValueMethodType.PercentComplete) कैसे निर्दिष्ट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
// अर्जित मूल्य विधि प्रकार को 'PercentComplete' सेट करें
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// परियोजना के साथ काम करें...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


