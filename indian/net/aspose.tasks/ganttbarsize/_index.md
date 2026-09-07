---
title: "एनम GanttBarSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GanttBarSize एनम। बिंदुओं में बार की ऊँचाई निर्दिष्ट करता है"
type: docs
weight: 700
url: /hi/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

बार की ऊँचाई को पॉइंट्स में निर्दिष्ट करता है।

```csharp
public enum GanttBarSize
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| BarSize6 | `0` | बार आकार 6 बिंदु। |
| BarSize8 | `1` | बार आकार 8 बिंदु। |
| BarSize10 | `2` | बार आकार 10 पॉइंट्स। |
| BarSize12 | `3` | बार आकार 12 पॉइंट्स। |
| BarSize14 | `4` | बार आकार 14 पॉइंट्स। |
| BarSize18 | `5` | बार आकार 18 पॉइंट्स। |
| BarSize24 | `6` | बार आकार 24 पॉइंट्स। |

## उदाहरण

दिखाता है कि Gantt चार्ट दृश्य की कुछ उपयोगी गुण कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// एक मान सेट करें जो दर्शाता है कि बार निकटतम दिन तक गोल होते हैं या नहीं
view.BarRounding = false;
// Gantt चार्ट में Gantt बार की ऊँचाई, पॉइंट्स में, सेट करें
view.BarSize = GanttBarSize.BarSize24;
// एक मान सेट करें जो दर्शाता है कि सारांश कार्य का विस्तार करते समय रोलअप बार छिपे होंगे या नहीं
view.HideRollupBarsWhenSummaryExpanded = true;
// गैर-कार्य समय का रंग सेट करें
view.NonWorkingTimeColor = Color.Azure;
// एक मान सेट करें जो दर्शाता है कि Gantt चार्ट पर बार को रोल अप किया जाना चाहिए या नहीं
view.RollUpGanttBars = true;
// एक मान सेट करें जो दर्शाता है कि Gantt चार्ट पर कार्य विभाजन दिखाए जाने चाहिए या नहीं
view.ShowBarSplits = true;
// एक मान सेट करें जो दर्शाता है कि Gantt चार्ट पर ड्रॉइंग्स दिखाए जाने चाहिए या नहीं
view.ShowDrawings = true;
// टाइमस्केल स्तर पर इकाइयों के बीच की दूरी को घटाने या बढ़ाने के लिए प्रतिशत सेट करें
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


