---
title: "Project.GetBaselineSaveTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। बेसलाइन सहेजने का समय लौटाता है"
type: docs
weight: 1090
url: /hi/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

बेसलाइन सहेजने का समय लौटाता है।

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| baselineNumber | BaselineType | बेसलाइन की संख्या [`BaselineType`](../../baselinetype/)। |

### रिटर्न वैल्यू

बेसलाइन की अंतिम सहेजने की तिथि और समय।

## टिप्पणियाँ

यदि बेसलाइन सहेजा नहीं गया तो DateTime.MinValue लौटाता है।

## उदाहरण

प्रोजेक्ट की बेसलाइन सहेजने के समय को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// बेसलाइन सहेजने का समय सेट करें
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### संबंधित देखें

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


