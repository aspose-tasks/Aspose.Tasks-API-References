---
title: "GanttChartView.Gridlines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। Gantt Chart व्यू की Gridlines की सूची प्राप्त या सेट करता है।"
type: docs
weight: 80
url: /hi/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

`Gridlines` की सूची प्राप्त या सेट करता है Gantt Chart व्यू की।

```csharp
public List<Gridlines> Gridlines { get; set; }
```

## उदाहरण

ग्रिडलाइन के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// व्यू की पहली ग्रिडलाइन को समायोजित करने देता है।
var gridlines = view.Gridlines[0];
// ग्रिडलाइन के बीच अंतराल निर्दिष्ट करने वाला संख्या 0 से 99 तक सेट करें।
gridlines.Interval = 2;
// द्वितीयक ग्रिडलाइन का रंग सेट करें।
gridlines.IntervalColor = Color.Red;
// द्वितीयक ग्रिडलाइन के लिए रेखा पैटर्न सेट करें
gridlines.IntervalPattern = LinePattern.Solid;
// सामान्य ग्रिडलाइन का रंग सेट करें
gridlines.NormalColor = Color.Blue;
// सामान्य ग्रिडलाइन के लिए रेखा पैटर्न सेट करें
gridlines.NormalPattern = LinePattern.CloseDot;
// ग्रिडलाइन प्रकार सेट करें
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


