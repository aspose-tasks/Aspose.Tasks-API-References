---
title: "GanttChartView.CustomBarStyles"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de GanttChartView. Obtiene una lista de estilos de barra personalizados específicos de tarea de la vista de diagrama de Gantt. GanttBarStyle"
type: docs
weight: 70
url: /es/net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

Obtiene una lista de estilos de barra personalizados específicos de tarea de la vista de diagrama de Gantt. [`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/).

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

## Ejemplos

Muestra cómo establecer estilos de barra personalizados en la vista de proyecto del diagrama de Gantt.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Agrega el estilo de barra personalizado a la colección de barras personalizadas de la vista del proyecto.
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

### Ver también

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


