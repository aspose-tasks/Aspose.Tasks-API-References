---
title: "क्लास TimescaleTier"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TimescaleTier क्लास। Gantt चार्ट पर टाइमस्केल का एकल स्तर दर्शाता है।"
type: docs
weight: 3450
url: /hi/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

गैंट चार्ट पर टाइमस्केल की एकल स्तर को दर्शाता है।

```csharp
public sealed class TimescaleTier
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | `TimescaleTier` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | `TimescaleTier` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | टियर के प्रत्येक समय अवधि में लेबल को कैसे संरेखित किया जाए, प्राप्त करता है या सेट करता है ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | टियर के लिए लेबल दिखाने वाले समय इकाई अंतराल को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान 1 है। |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए कॉलबैक फ़ंक्शन प्राप्त करता है या सेट करता है। |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | टाइमस्केल टियर के लिए तिथि लेबल [`DateLabel`](../datelabel/) प्राप्त करता है या सेट करता है। |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | एक फ़्लैग प्राप्त करता है या सेट करता है जो निर्धारित करता है कि जब समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाएँ या नहीं। यदि मान 'true' है, तो जब समय अवधि कई पृष्ठों में फैली हो, तो अवधि के तिथि लेबल प्रत्येक पृष्ठ पर रेंडर होते हैं। यदि मान 'false' है, तो तिथि लेबल केवल एक बार रेंडर होता है, जो [`Alignment`](./alignment/) प्रॉपर्टी के मान के अनुसार होता है। |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | टाइमस्केल टियर के लिए टाइमस्केल यूनिट [`TimescaleUnit`](../timescaleunit/) प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान [`Days`](../timescaleunit/) है। |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | टियर लेबल को वित्तीय वर्ष पर आधारित करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


