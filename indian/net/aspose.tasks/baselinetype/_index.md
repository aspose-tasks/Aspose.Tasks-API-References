---
title: "Enum BaselineType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BaselineType enum. वैरिएंस मानों की गणना के लिए उपयोग किए जाने वाले बेसलाइन प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

वैरिएंस मानों की गणना के लिए उपयोग किए जाने वाले बेसलाइन प्रकार को निर्दिष्ट करता है।

```csharp
public enum BaselineType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | इंगित करता है कि फ़ील्ड मूल प्रोजेक्ट फ़ाइल में परिभाषित नहीं था। |
| Baseline | `0` | बेसलाइन प्रकार को इंगित करता है। |
| Baseline1 | `1` | बेसलाइन1 प्रकार को इंगित करता है। |
| Baseline2 | `2` | बेसलाइन2 प्रकार को इंगित करता है। |
| Baseline3 | `3` | बेसलाइन3 प्रकार को इंगित करता है। |
| Baseline4 | `4` | बेसलाइन4 प्रकार को इंगित करता है। |
| Baseline5 | `5` | बेसलाइन5 प्रकार को इंगित करता है। |
| Baseline6 | `6` | बेसलाइन6 प्रकार को इंगित करता है। |
| Baseline7 | `7` | बेसलाइन7 प्रकार को इंगित करता है। |
| Baseline8 | `8` | बेसलाइन8 प्रकार को इंगित करता है। |
| Baseline9 | `9` | बेसलाइन9 प्रकार को इंगित करता है। |
| Baseline10 | `10` | बेसलाइन10 प्रकार को इंगित करता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि प्रोजेक्ट के लिए बेसलाइन (BaselineType.Baseline) कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
// पूरे प्रोजेक्ट के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड सहेजें।
project.SetBaseline(BaselineType.Baseline);
// प्रोजेक्ट की बेसलाइन के साथ काम करें...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


