---
title: "Enum YearLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.YearLabelDisplay enum. वर्ष लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।"
type: docs
weight: 3680
url: /hi/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

वर्ष लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।

```csharp
public enum YearLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Y | `0` | MS Project में वर्षों की सूची को 'mo' के रूप में सेट करता है। |
| Yr | `1` | MS Project में वर्षों की सूची को 'mon' के रूप में सेट करता है। |
| Year | `2` | MS Project में वर्षों की सूची को महीने के रूप में सेट करता है। |

## उदाहरण

प्रोजेक्ट की डिस्प्ले विकल्पों में वर्ष लेबल सेट करने का तरीका दिखाता है (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// वर्ष लेबल कैसे प्रदर्शित किया जाता है, सेट करें
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


