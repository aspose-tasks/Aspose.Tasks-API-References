---
title: "SaveOptions.StartDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। रेंडरिंग शुरू करने की तिथि को प्राप्त करता है या सेट करता है।"
type: docs
weight: 170
url: /hi/net/aspose.tasks.saving/saveoptions/startdate/
---
## SaveOptions.StartDate property

रेंडरिंग शुरू करने की तिथि को प्राप्त करता है या सेट करता है।

```csharp
public DateTime StartDate { get; set; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


