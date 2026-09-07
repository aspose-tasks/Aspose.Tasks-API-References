---
title: "GanttChartView.TopTimescaleTier"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। व्यू के टॉप टाइमस्केल टियर की सेटिंग्स प्राप्त या सेट करता है। TimescaleTier"
type: docs
weight: 190
url: /hi/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

प्राप्त करता है या सेट करता है व्यू के शीर्ष टाइमस्केल टियर की सेटिंग्स। [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
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

टाइमस्केल टियर लेबल को कस्टमाइज़ करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// टास्क लिंक जोड़ें
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// टाइमस्केल टियर्स को ट्यून करें

// शीर्ष टियर को ट्यून करें
// Gantt चार्ट व्यू का शीर्ष टाइमस्केल टियर सेट करें।
view.MiddleTimescaleTier = new TimescaleTier();
// टाइमस्केल टियर के लिए टाइमस्केल यूनिट <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> सेट करें।
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// टियर के लिए लेबल दिखाने वाले समय इकाई अंतराल को सेट करें।
view.MiddleTimescaleTier.Count = 1;
// टाइमस्केल टियर के लिए तिथि लेबल <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> सेट करें।
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// टियर के प्रत्येक समय अवधि में लेबल को कैसे संरेखित किया जाए, सेट करें (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// टियर में समय अवधि को अलग करने वाले टिक मार्क दिखाने चाहिए या नहीं, यह दर्शाने के लिए मान सेट करें।
view.MiddleTimescaleTier.ShowTicks = true;
// वित्तीय वर्ष के आधार पर टियर लेबल सेट करने के लिए मान निर्धारित करें।
view.MiddleTimescaleTier.UsesFiscalYear = true;

// बेहतर दृश्यता के लिए जोड़ा गया
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// मध्य टियर की तिथियों को अनुकूलित करें
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// व्यू में परिभाषित टाइमस्केल सेटिंग्स (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) का उपयोग करके टाइमस्केल रेंडर करने के लिए 'Timescale.DefinedInView' विकल्प का उपयोग करें।
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### संबंधित देखें

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


