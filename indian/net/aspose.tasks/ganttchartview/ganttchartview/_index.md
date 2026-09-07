---
title: "GanttChartView.GanttChartView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView कंस्ट्रक्टर। GanttChartView क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

[`GanttChartView`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public GanttChartView()
```

## उदाहरण

टाइमस्केल टियर्स को संशोधित करने का तरीका दिखाता है।

```csharp
var project = new Project();

// Gantt Chart View को इनिट करें
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// टाइम स्केल काउंट सेट करें
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// प्रोजेक्ट में Gantt Chart View जोड़ें
project.Views.Add(view);

// प्रोजेक्ट में कुछ परीक्षण डेटा जोड़ें
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// 'Timescale.DefinedInView' विकल्प का उपयोग करके टाइमस्केल सेटिंग्स (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) के आधार पर टाइमस्केल रेंडर करें।
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### संबंधित देखें

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


