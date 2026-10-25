---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि महत्वपूर्ण कार्यों को लाल रंग में दिखाया जाना चाहिए या नहीं; डिफ़ॉल्ट मान FALSE है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि महत्वपूर्ण कार्यों को लाल रंग में दिखाया जाए या नहीं (डिफ़ॉल्ट मान FALSE है)।

```csharp
public bool MarkCriticalTasks { get; set; }
```

## उदाहरण

दिखाता है कि इमेज फ़ाइल फ़ॉर्मेट में सहेजते समय महत्वपूर्ण कार्यों को कैसे प्रिंट किया जाए।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

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


