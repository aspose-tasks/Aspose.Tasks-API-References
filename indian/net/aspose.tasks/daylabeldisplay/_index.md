---
title: "Enum DayLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DayLabelDisplay enum. दिन लेबल के प्रदर्शित होने का तरीका निर्दिष्ट करता है"
type: docs
weight: 440
url: /hi/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

निर्दिष्ट करता है कि दिन लेबल कैसे प्रदर्शित होता है।

```csharp
public enum DayLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| D | `0` | MS Project में Days सूची को d के रूप में सेट करता है। |
| Dy | `1` | MS Project में Days सूची को dy के रूप में सेट करता है। |
| Day | `2` | MS Project में Days सूची को day के रूप में सेट करता है। |

## उदाहरण

प्रोजेक्ट के डिस्प्ले विकल्पों में दिन लेबल सेट करने का तरीका दिखाता है (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// दिन लेबल कैसे प्रदर्शित होता है, इसे सेट करें।
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


