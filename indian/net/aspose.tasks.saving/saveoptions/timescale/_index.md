---
title: "SaveOptions.Timescale"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है Timescale मान जिसे प्रोजेक्ट को ग्राफ़िकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) के रेंडरिंग को नियंत्रित करने के लिए उपयोग किया जाता है।"
type: docs
weight: 200
url: /hi/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

प्राप्त करता है या सेट करता है `Timescale` मान जिसे प्रोजेक्ट को ग्राफ़िकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) के रेंडरिंग को नियंत्रित करने के लिए उपयोग किया जाता है।

```csharp
public Timescale Timescale { get; set; }
```

## उदाहरण

दिखाता है कि रेंडर करने के लिए न्यूनतम समय अवधि कैसे सेट की जाए। डिफ़ॉल्ट मान है <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// एक पृष्ठ की इमेज में सहेजें (डिफ़ॉल्ट रूप से Timescale.days)।
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// एक पृष्ठ की इमेज में सहेजें (Timescale.ThirdsOfMonths)।
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// एक पृष्ठ की इमेज में सहेजें (Timescale.Months)।
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

सेव विकल्पों के माध्यम से टाइमस्केल टियर्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// Gantt Chart दृश्य के टाइमस्केल टियर्स को सेट करें
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// परियोजना को छवि के रूप में सहेजें
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
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

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


