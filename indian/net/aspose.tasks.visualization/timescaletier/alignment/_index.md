---
title: "TimescaleTier.Alignment"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TimescaleTier प्रॉपर्टी। टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, यह प्राप्त करता है या सेट करता है HorizontalStringAlignment।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/timescaletier/alignment/
---
## TimescaleTier.Alignment property

टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, यह प्राप्त करता है या सेट करता है ([`HorizontalStringAlignment`](../../horizontalstringalignment/)).

```csharp
public HorizontalStringAlignment Alignment { get; set; }
```

## उदाहरण

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

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


