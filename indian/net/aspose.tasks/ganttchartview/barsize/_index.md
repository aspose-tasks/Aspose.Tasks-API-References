---
title: "GanttChartView.BarSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। Gantt Chart में Gantt बार की ऊँचाई पॉइंट्स में प्राप्त करता है या सेट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/ganttchartview/barsize/
---
## GanttChartView.BarSize property

Gantt Chart में Gantt बारों की ऊँचाई (पॉइंट्स में) को प्राप्त या सेट करता है।

```csharp
public GanttBarSize BarSize { get; set; }
```

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

* enum [GanttBarSize](../../ganttbarsize/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


