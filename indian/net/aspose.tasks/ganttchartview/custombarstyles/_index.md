---
title: "GanttChartView.CustomBarStyles"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। Gantt Chart दृश्य के लिए कस्टम टास्क-विशिष्ट बार शैलियों की सूची प्राप्त करता है। GanttBarStyle"
type: docs
weight: 70
url: /hi/net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

Gantt Chart दृश्य के लिए कस्टम टास्क-विशिष्ट बार शैलियों की सूची प्राप्त करता है। [`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/).

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

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

### संबंधित देखें

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


