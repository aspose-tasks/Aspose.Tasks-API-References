---
title: "क्लास Gridlines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.Gridlines क्लास। यह GanttChart दृश्य में दिखाई देने वाली ग्रिडलाइन का प्रतिनिधित्व करता है"
type: docs
weight: 3120
url: /hi/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

गैंटचार्ट दृश्य में दिखाई देने वाली ग्रिडलाइन को दर्शाता है।

```csharp
public class Gridlines
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Gridlines](gridlines/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | ग्रिडलाइन के बीच अंतराल निर्दिष्ट करने वाले 0 से 99 तक की संख्या को प्राप्त करता है या सेट करता है। |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | द्वितीयक ग्रिडलाइन का रंग प्राप्त करता है या सेट करता है। |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | द्वितीयक ग्रिडलाइन के लिए रेखा पैटर्न प्राप्त करता है या सेट करता है। |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | सामान्य ग्रिडलाइन का रंग प्राप्त करता है या सेट करता है। |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | सामान्य ग्रिडलाइन के लिए रेखा पैटर्न प्राप्त करता है या सेट करता है। |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | ग्रिडलाइन प्रकार प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


