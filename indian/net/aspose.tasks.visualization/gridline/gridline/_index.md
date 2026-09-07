---
title: "Gridline.Gridline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Gridline कंस्ट्रक्टर। Gridline क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

[`Gridline`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public Gridline()
```

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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


