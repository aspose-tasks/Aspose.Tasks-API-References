---
title: "Enum GanttBarMiddleShape"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. बार के मध्य आकार को निर्दिष्ट करता है।"
type: docs
weight: 3050
url: /hi/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

बार के मध्य आकार को निर्दिष्ट करता है।

```csharp
public enum GanttBarMiddleShape
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| LineBottom | `7` | नीचे संरेखित रेखा आकार को दर्शाता है। |
| LineMiddle | `6` | केंद्र संरेखित रेखा आकार को दर्शाता है। |
| LineTop | `5` | ऊपर संरेखित रेखा आकार को दर्शाता है। |
| None | `0` | खाली आकार दर्शाता है। |
| RectangleBar | `1` | पूर्ण ऊँचाई वाले आयताकार बार आकार को दर्शाता है। |
| RectangleBottom | `4` | निचले संरेखित आधी ऊँचाई वाले आयताकार बार आकार को दर्शाता है। |
| RectangleMiddle | `3` | केन्द्र-संरेखित 1/3 ऊँचाई वाले आयताकार बार आकार को दर्शाता है। |
| RectangleTop | `2` | ऊपर संरेखित आधा-ऊँचाई आयत बार आकार को दर्शाता है। |

## उदाहरण

दिखाता है कि Gantt चार्ट प्रोजेक्ट व्यू की कस्टम बार शैलियों को कैसे सेट किया जाए।

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // कस्टम बार शैली को प्रोजेक्ट व्यू के कस्टम बार संग्रह में जोड़ें।
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


