---
title: "SaveOptions.Gridlines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्रोजेक्ट व्यू में दिखाई देने वाली Gridline की सूची प्राप्त करता है या सेट करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

प्रोजेक्ट व्यू में दिखाई देने वाली [`Gridline`](../../../aspose.tasks.visualization/gridline/) की सूची प्राप्त करता है या सेट करता है।

```csharp
public List<Gridline> Gridlines { get; set; }
```

## उदाहरण

दिखाता है कि लेआउट को अलग-अलग फ़ाइलों में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// प्रोजेक्ट लेआउट को अलग-अलग फ़ाइलों में सहेजें
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### संबंधित देखें

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


