---
title: "Enum PageSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageSize enum. पेज आकार को निर्दिष्ट करता है।"
type: docs
weight: 3250
url: /hi/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

पेज आकार को निर्दिष्ट करता है।

```csharp
public enum PageSize
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Letter | `0` | Letter पेज का आकार पॉइंट्स में 792 × 612 |
| Ledger | `1` | Ledger पेज का आकार पॉइंट्स में 1224 × 792 |
| A0 | `2` | A0 पेज का आकार पॉइंट्स में 3371 × 2384 |
| A1 | `3` | A1 पेज का आकार पॉइंट्स में 2384 × 1685 |
| A2 | `4` | A2 पेज का आकार पॉइंट्स में 1684 × 1190 |
| A3 | `5` | A3 पेज का आकार पॉइंट्स में 1190 × 842 |
| A4 | `6` | A4 पेज का आकार पॉइंट्स में 842 × 595 |
| DefinedInView | `7` | View के [`PageSettings`](../pagesettings/) में परिभाषित पृष्ठ आकार का उपयोग करें (View.PageInfo.PageSettings). |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


