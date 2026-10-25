---
title: "एनम MonthLabelDisplay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MonthLabelDisplay enum. निर्दिष्ट करता है कि महीने का लेबल कैसे प्रदर्शित होता है"
type: docs
weight: 1060
url: /hi/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

माह लेबल कैसे प्रदर्शित होता है, यह निर्दिष्ट करता है।

```csharp
public enum MonthLabelDisplay
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Mo | `0` | MS Project में महीनों की सूची को mo के रूप में सेट करता है। |
| Mon | `1` | MS Project में महीनों की सूची को mon के रूप में सेट करता है। |
| Month | `2` | MS Project में महीनों की सूची को month के रूप में सेट करता है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट के डिस्प्ले विकल्पों में महीने का लेबल कैसे सेट किया जाए (केस 1)।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// महीने का लेबल कैसे प्रदर्शित होता है, सेट करें
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


