---
title: "Gridlines.NormalPattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Gridlines प्रॉपर्टी। सामान्य ग्रिडलाइन के लिए लाइन पैटर्न प्राप्त या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/gridlines/normalpattern/
---
## Gridlines.NormalPattern property

सामान्य ग्रिडलाइन के लिए रेखा पैटर्न प्राप्त करता है या सेट करता है।

```csharp
public LinePattern NormalPattern { get; set; }
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

* enum [LinePattern](../../linepattern/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


