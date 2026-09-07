---
title: "GanttChartView.RollUpGanttBars"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि Gantt Chart पर बार को रोल अप करना आवश्यक है या नहीं"
type: docs
weight: 130
url: /hi/net/aspose.tasks/ganttchartview/rollupganttbars/
---
## GanttChartView.RollUpGanttBars property

Gantt Chart पर बारों को रोल अप करने का संकेत देने वाले मान को प्राप्त या सेट करता है।

```csharp
public bool RollUpGanttBars { get; set; }
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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


