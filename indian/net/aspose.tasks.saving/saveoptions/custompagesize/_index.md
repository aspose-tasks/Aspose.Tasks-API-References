---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह कस्टम पेज आकार को पॉइंट्स में प्राप्त करता है या सेट करता है (1 पॉइंट = 1/72 इंच)।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

कस्टम पेज आकार को पॉइंट्स में प्राप्त करता है या सेट करता है (1 पॉइंट = इंच का 1/72)।

```csharp
public SizeF CustomPageSize { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को PDF में सहेजते समय कस्टम पेज आकार कैसे सेट किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


