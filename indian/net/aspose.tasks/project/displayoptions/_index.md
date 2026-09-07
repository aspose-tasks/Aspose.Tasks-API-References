---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। ProjectDisplayOptions क्लास का एक इंस्टेंस प्राप्त करता है"
type: docs
weight: 380
url: /hi/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

[`ProjectDisplayOptions`](../../projectdisplayoptions/) क्लास का एक इंस्टेंस प्राप्त करता है।

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट के डिस्प्ले विकल्पों को कैसे ट्यून करें।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// प्रोजेक्ट द्वारा मैन्युअल रूप से निर्धारित कार्य में संभावित शेड्यूलिंग टकराव की पहचान होने पर चेतावनियाँ दिखाने के लिए मान सेट करें।
// यह विकल्प प्रोजेक्ट 2010 संस्करण और बाद के संस्करणों के लिए उपलब्ध है।
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### संबंधित देखें

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


