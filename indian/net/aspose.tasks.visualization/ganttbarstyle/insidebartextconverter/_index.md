---
title: "GanttBarStyle.InsideBarTextConverter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttBarStyle प्रॉपर्टी। टास्क बार के अंदर रेंडर करने के लिए टेक्स्ट प्राप्त करने वाले यूज़र-डिफाइंड कनवर्टर को प्राप्त करता है या सेट करता है। InsideField प्रॉपर्टी के मान को ओवरराइड करता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks.visualization/ganttbarstyle/insidebartextconverter/
---
## GanttBarStyle.InsideBarTextConverter property

टास्क बार के अंदर रेंडर करने के लिए टेक्स्ट प्राप्त करने वाले यूज़र-डिफाइंड कनवर्टर को प्राप्त करता है या सेट करता है। [`InsideField`](../insidefield/) प्रॉपर्टी के मान को ओवरराइड करता है।

```csharp
public TaskBarTextConverter InsideBarTextConverter { get; set; }
```

## टिप्पणियाँ

MPP फ़ॉर्मेट में सहेजा नहीं जाता है।

## उदाहरण

दिखाता है कि Gantt चार्ट व्यू की कस्टम बार शैलियों का उपयोग कैसे किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// बार शैलियाँ या तो टास्क-विशिष्ट हो सकती हैं (GanttChartView.CustomBarStyles में स्थित)।
// या श्रेणी-विशिष्ट (GanttChartView.BarStyles में स्थित)।
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // प्रदर्शन के उद्देश्य से हम टास्क जिसका यूनिक आईडी = 4 है, की शैली को संशोधित कर रहे हैं।
    // यहाँ हम फ़ील्ड (TaskName) को टास्क बार के बाएँ तरफ रेंडर करने के लिए सेट करते हैं।
    ganttBarStyle.LeftField = Field.TaskName;
    // यहाँ हम कस्टम कन्वर्टर सेट करते हैं ताकि यह नियंत्रित किया जा सके कि टास्क बार के अंदर कौन सा टेक्स्ट रेंडर होना चाहिए।
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // प्रदर्शन के उद्देश्य से हम माइलस्टोन टास्क पर लागू शैलियों को संशोधित कर रहे हैं।

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### संबंधित देखें

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


