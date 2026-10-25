---
title: "Enum WeekLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WeekLabelDisplay enum. सप्ताह लेबल के प्रदर्शित होने का तरीका निर्दिष्ट करता है"
type: docs
weight: 3560
url: /hi/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

सप्ताह लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।

```csharp
public enum WeekLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| W | `0` | \"w\" लेबल। |
| Wk | `1` | \"wk\" लेबल। |
| Week | `2` | \"week\" लेबल। |

## उदाहरण

प्रोजेक्ट के डिस्प्ले विकल्पों में सप्ताह लेबल सेट करने का तरीका दिखाता है (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// सप्ताह लेबल कैसे प्रदर्शित होता है, इसे सेट करें।
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


