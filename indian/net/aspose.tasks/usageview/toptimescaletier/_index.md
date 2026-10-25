---
title: "UsageView.TopTimescaleTier"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "UsageView प्रॉपर्टी। प्राप्त करता है या सेट करता है व्यूज़ के शीर्ष टाइमस्केल टियर की सेटिंग्स। TimescaleTier"
type: docs
weight: 80
url: /hi/net/aspose.tasks/usageview/toptimescaletier/
---
## UsageView.TopTimescaleTier property

प्राप्त करता है या सेट करता है व्यू के शीर्ष टाइमस्केल टियर की सेटिंग्स। [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## उदाहरण

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

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


