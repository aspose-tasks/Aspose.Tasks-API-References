---
title: "GanttChartView.CustomBarStyles"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Chart görünümünün özel görev‑spesifik çubuk stillerinin bir listesini alır. GanttBarStyle"
type: docs
weight: 70
url: /tr/net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

Gantt Chart görünümünün özel görev‑spesifik çubuk stillerinin bir listesini alır. [`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/).

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

## Örnekler

Gantt Şeması proje görünümünün özel çubuk stillerinin nasıl ayarlanacağını gösterir.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Özel çubuk stilini proje görünümünün özel çubuk koleksiyonuna ekleyin
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

### Ayrıca Bakınız

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


