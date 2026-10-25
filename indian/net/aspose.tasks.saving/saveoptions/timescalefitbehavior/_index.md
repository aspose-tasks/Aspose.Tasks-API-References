---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। एक व्यवहार प्राप्त करता है या सेट करता है जो यह निर्धारित करता है कि टाइमस्केल के दाएँ अंत को पृष्ठ के अंत के साथ कैसे संरेखित किया जाए।"
type: docs
weight: 210
url: /hi/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

टाइमस्केल के दाएँ अंत को पृष्ठ के अंत के साथ संरेखित करने के तरीके को परिभाषित करने वाले व्यवहार को प्राप्त करता है या सेट करता है।

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## उदाहरण

दिखाता है कि TimescaleFitBehavior का उपयोग करके Gantt चार्ट का टाइमस्केल अंतिम पेज के अंत तक कैसे फिट करें।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### संबंधित देखें

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


