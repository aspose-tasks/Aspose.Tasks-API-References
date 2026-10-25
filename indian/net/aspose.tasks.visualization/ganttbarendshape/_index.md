---
title: "Enum GanttBarEndShape"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. बार और प्रोग्रेस लाइनों में प्रोग्रेस पॉइंट्स में अंत आकार का प्रतिनिधित्व करता है।"
type: docs
weight: 3030
url: /hi/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

बार और प्रोग्रेस लाइनों में प्रोग्रेस पॉइंट्स के अंत आकार का प्रतिनिधित्व करता है।

```csharp
public enum GanttBarEndShape
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| ArrowDown | `14` | नीचे की ओर इशारा करने वाला तीर Gantt बार अंत आकार को दर्शाता है। |
| ArrowUp | `8` | ऊपर की ओर इशारा करने वाला तीर Gantt बार अंत आकार को दर्शाता है। |
| CaretDownTop | `9` | बार के ऊपर आधे हिस्से पर नीचे की ओर इशारा करने वाला केयरट Gantt बार अंत आकार को दर्शाता है। |
| CaretUpBottom | `10` | बार के नीचे आधे हिस्से पर ऊपर की ओर इशारा करने वाला केयरट Gantt बार अंत आकार को दर्शाता है। |
| Circle | `19` | वृत्त Gantt बार अंत आकार को दर्शाता है। |
| CircleArrowDown | `18` | नीचे की ओर इशारा करने वाला घेराव वाला तीर Gantt बार अंत आकार को दर्शाता है। |
| CircleArrowUp | `17` | ऊपर की ओर इशारा करने वाला घेराव वाला तीर Gantt बार अंत आकार को दर्शाता है। |
| CircleDiamond | `13` | घेराव वाला हीरा Gantt बार अंत आकार को दर्शाता है। |
| CircleTriangleDown | `16` | नीचे की ओर इशारा करने वाला घेराव वाला त्रिकोण Gantt बार अंत आकार को दर्शाता है। |
| CircleTriangleUp | `15` | ऊपर की ओर इशारा करने वाला घेराव वाला त्रिकोण Gantt बार अंत आकार को दर्शाता है। |
| Diamond | `3` | हीरा Gantt बार अंत आकार को दर्शाता है। |
| HouseDown | `2` | उलटा घर Gantt बार अंत आकार को दर्शाता है। |
| HouseUp | `1` | घर Gantt बार अंत आकार को दर्शाता है। |
| LeftBracket | `21` | बायाँ कोष्ठक Gantt बार अंत आकार को दर्शाता है। |
| LeftFade | `23` | बायाँ फेड Gantt बार अंत आकार को दर्शाता है। |
| LineShape | `11` | रेखा Gantt बार अंत आकार को दर्शाता है। |
| NoBarEndShape | `0` | कोई नहीं Gantt बार अंत आकार को दर्शाता है। |
| RightBracket | `22` | दायाँ कोष्ठक Gantt बार अंत आकार को दर्शाता है। |
| RightFade | `24` | दायाँ फेड Gantt बार अंत आकार को दर्शाता है। |
| Square | `12` | वर्ग Gantt बार अंत आकार को दर्शाता है। |
| Star | `20` | तारा Gantt बार अंत आकार को दर्शाता है। |
| TriangleDown | `5` | नीचे की ओर इशारा करने वाला त्रिकोण Gantt बार अंत आकार को दर्शाता है। |
| TriangleLeft | `7` | बाएँ की ओर इशारा करने वाले त्रिकोण को दर्शाता है, जो Gantt बार के अंत के आकार को दर्शाता है। |
| TriangleRight | `6` | दाएँ की ओर इशारा करने वाले त्रिकोण को दर्शाता है, जो Gantt बार के अंत के आकार को दर्शाता है। |
| TriangleUp | `4` | ऊपर की ओर इशारा करने वाला घेराव वाला त्रिकोण Gantt बार अंत आकार को दर्शाता है। |

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


