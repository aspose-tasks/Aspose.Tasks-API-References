---
title: "क्लास Gridline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.Gridline क्लास। वह क्षैतिज या लंबवत रेखा जो प्रोजेक्ट व्यू में दिखाई देती है।"
type: docs
weight: 3100
url: /hi/net/aspose.tasks.visualization/gridline/
---
## Gridline class

प्रोजेक्ट दृश्य में दिखाई देने वाली क्षैतिज या लंबवत रेखा।

```csharp
public class Gridline
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Gridline](gridline/)() | `Gridline` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | ग्रिडलाइन का [`Color`](./color/) प्राप्त करता है या सेट करता है। |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | ग्रिडलाइन का प्रकार ([`GridlineType`](./gridlinetype/)) प्राप्त करता है या सेट करता है। |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | ग्रिडलाइन का [`LinePattern`](../linepattern/) प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | `Gridline` क्लास के इंस्टेंस के लिए हैश कोड वैल्यू लौटाता है। |

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


