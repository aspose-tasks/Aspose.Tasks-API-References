---
title: "एनम HourLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.HourLabelDisplay एनम। घंटे लेबल के प्रदर्शित होने का तरीका निर्दिष्ट करता है।"
type: docs
weight: 820
url: /hi/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

घंटा लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।

```csharp
public enum HourLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| H | `0` | "h" लेबल। |
| Hr | `1` | "hr" लेबल। |
| Hour | `2` | "hour(s)" लेबल। |

## उदाहरण

दिखाता है कि प्रोजेक्ट की डिस्प्ले विकल्पों में घंटे लेबल को कैसे सेट करें (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// घंटे लेबल के प्रदर्शित होने का तरीका सेट करें।
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


