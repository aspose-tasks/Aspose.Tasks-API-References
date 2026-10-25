---
title: "Enum MinuteLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MinuteLabelDisplay enum. मिनट लेबल कैसे प्रदर्शित होता है, इसे निर्दिष्ट करता है।"
type: docs
weight: 1030
url: /hi/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

मिनट लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।

```csharp
public enum MinuteLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| M | `0` | MS Project में मिनट सूची को m के रूप में सेट करता है। |
| Min | `1` | MS Project में मिनट सूची को min के रूप में सेट करता है। |
| Minute | `2` | MS Project में मिनट सूची को minute के रूप में सेट करता है। |

## उदाहरण

प्रोजेक्ट की डिस्प्ले विकल्पों में मिनट लेबल सेट करने का तरीका दर्शाता है (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// मिनट लेबल कैसे प्रदर्शित होता है, इसे सेट करें
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


