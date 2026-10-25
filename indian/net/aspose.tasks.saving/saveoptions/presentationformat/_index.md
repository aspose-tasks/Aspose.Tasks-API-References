---
title: "SaveOptions.PresentationFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। उस PresentationFormat को प्राप्त करता है या सेट करता है जिसमें दस्तावेज़ सहेजा जाएगा।"
type: docs
weight: 140
url: /hi/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

दस्तावेज़ को सहेजने के लिए `PresentationFormat` को प्राप्त करता है या सेट करता है।

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

व्यू सेटिंग्स में परिभाषित टाइमस्केल सेटिंग्स के साथ टास्क उपयोग दृश्य को रेंडर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// SaveOptions को परिभाषित करें और निर्दिष्ट करें कि TaskUsageView टाइमस्केल सेटिंग्स का उपयोग किया जाना चाहिए।
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### संबंधित देखें

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


