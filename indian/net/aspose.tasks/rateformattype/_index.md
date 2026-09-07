---
title: "एनम RateFormatType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RateFormatType एनम। Microsoft Project द्वारा दर प्रदर्शित करने के लिए उपयोग की जाने वाली इकाइयों को निर्दिष्ट करता है"
type: docs
weight: 1640
url: /hi/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

माइक्रोसॉफ्ट प्रोजेक्ट द्वारा दर प्रदर्शित करने के लिए उपयोग किए जाने वाले इकाइयों को निर्दिष्ट करता है।

```csharp
public enum RateFormatType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था। |
| Minute | `0` | मिनट ("min") |
| Hour | `1` | घंटा ("hr") |
| Day | `2` | दिन ("day") |
| Week | `3` | सप्ताह ("wk") |
| Month | `4` | माह ("mo") |
| Year | `5` | वर्ष ("yr") |
| MaterialResourceRate | `6` | सामग्री संसाधन दर (खाली) |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि Rsc.StandardRateFormat प्रॉपर्टी को कैसे पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


