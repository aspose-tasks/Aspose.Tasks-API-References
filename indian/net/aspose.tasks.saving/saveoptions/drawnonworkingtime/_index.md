---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं; डिफ़ॉल्ट मान TRUE है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)।

```csharp
public bool DrawNonWorkingTime { get; set; }
```

## उदाहरण

दिखाता है कि कैसे एक मान सेट किया जाए जो संकेत देता है कि सारांश कार्य बार पर उपकार्य को रोल अप किया जाना चाहिए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // या
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


