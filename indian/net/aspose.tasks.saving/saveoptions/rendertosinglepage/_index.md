---
title: "SaveOptions.RenderToSinglePage"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो दर्शाता है कि जब प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजा जाता है तो उसे एक ही पेज पर रेंडर किया जाना चाहिए या नहीं। पेज आकार बदल दिया जाएगा ताकि रेंडर किया गया प्रोजेक्ट एक पेज में फिट हो सके।"
type: docs
weight: 150
url: /hi/net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजते समय प्रोजेक्ट को एक ही पेज पर रेंडर किया जाए या नहीं। पेज आकार बदल दिया जाएगा ताकि रेंडर किया गया प्रोजेक्ट एक पेज में फिट हो सके।

```csharp
public bool RenderToSinglePage { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट के चयनित पेजों को PDF फ़ाइल में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// आइए जांचते हैं कि कितने पेज निर्यात किए जा सकते हैं
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

दिखाता है कि कैसे RenderToSinglePage प्रॉपर्टी का उपयोग करके यह निर्दिष्ट किया जाए कि प्रोजेक्ट को 1-पेज PDF में सहेजा जाना चाहिए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.TaskUsage;
options.Timescale = Timescale.DefinedInView;
options.RenderToSinglePage = true;
options.StartDate = new DateTime(2012, 12, 22);
options.EndDate = new DateTime(2013, 05, 10);

project.Save(OutDir + "WorkWithRenderToSinglePage_out.pdf", options);
```

दिखाता है कि चयनित पेजों को छवि के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

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


