---
title: "Enum GridlineType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.GridlineType enum. ग्रिडलाइन का प्रकार"
type: docs
weight: 3110
url: /hi/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

ग्रिडलाइन का प्रकार।

```csharp
public enum GridlineType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| GanttRow | `0` | Gantt पंक्ति ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| TopTierColumn | `1` | ऊपरी स्तर कॉलम ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| BottomTierColumn | `2` | निचले स्तर कॉलम ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| SheetRow | `3` | शीट पंक्ति ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| SheetColumn | `4` | शीट कॉलम ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| UsageRow | `5` | उपयोग पंक्ति ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| UsageColumn | `6` | उपयोग कॉलम ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |
| GanttTitleVertical | `7` | Gantt शीर्षक की लंबवत ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttTitleHorizontal | `8` | Gantt शीर्षक की क्षैतिज ग्रिड लाइन प्रकार को दर्शाता है। |
| BarRows | `9` | बार पंक्तियों की ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttProjectStart | `10` | Gantt प्रोजेक्ट शुरूआत ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttProjectFinish | `11` | Gantt प्रोजेक्ट समाप्ति ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttStatusDate | `12` | Gantt स्थिति तिथि ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttCurrentDate | `13` | Gantt वर्तमान तिथि ग्रिड लाइन प्रकार को दर्शाता है। |
| GanttPageBreaks | `14` | Gantt पेज ब्रेक्स ग्रिड लाइन प्रकार को दर्शाता है। |
| MiddleTierColumn | `15` | मिडल टियर कॉलम ग्रिड लाइन प्रकार की ग्रिडलाइन को दर्शाता है। |

## उदाहरण

विज़ुअल फ़ॉर्मैट्स में सहेजते समय ग्रिडलाइन के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // ग्रिडलाइन का प्रकार सेट करें (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // ग्रिडलाइन का <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> सेट करें
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


