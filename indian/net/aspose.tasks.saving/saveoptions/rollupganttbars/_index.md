---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो दर्शाता है कि सारांश टास्क बार पर सबटास्क को चिह्नित किया जाना चाहिए या नहीं। सबटास्क के लिए Rollup फ़ील्ड यह संकेत देता है कि सबटास्क Gantt बार की जानकारी सारांश टास्क बार में रोल अप होगी या नहीं। सारांश टास्क के लिए Rollup फ़ील्ड यह दर्शाता है कि सारांश टास्क बार रोल अप बार दिखाता है या नहीं। किसी भी सबटास्क को रोल अप करने के लिए आपको सारांश टास्क के लिए Rollup फ़ील्ड को Yes पर सेट करना आवश्यक है।"
type: docs
weight: 160
url: /hi/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि सारांश कार्य बार पर उप‑कार्य को चिह्नित किया जाए या नहीं। उप‑कार्य के लिए, Rollup फ़ील्ड यह दर्शाता है कि उप‑कार्य के गैंट बार की जानकारी सारांश कार्य बार में रोल‑अप होगी या नहीं। सारांश कार्यों के लिए, Rollup फ़ील्ड यह दर्शाता है कि सारांश कार्य बार रोल‑अप बार दिखाता है या नहीं। किसी भी उप‑कार्य को उनके पास रोल‑अप करने के लिए आपको सारांश कार्यों के लिए Rollup फ़ील्ड को Yes पर सेट करना आवश्यक है।

```csharp
public bool RollUpGanttBars { get; set; }
```

## टिप्पणियाँ

केवल तब लागू होता है जब Gantt चार्ट व्यू रेंडर किया जाता है।

## उदाहरण

दिखाता है कि कैसे एक मान सेट किया जाए जो संकेत देता है कि सारांश कार्य बार पर उपकार्य को रोल अप किया जाना चाहिए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // या
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


