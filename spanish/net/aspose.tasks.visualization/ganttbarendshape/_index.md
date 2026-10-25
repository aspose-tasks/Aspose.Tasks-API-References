---
title: "Enum GanttBarEndShape"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Representa la forma final en barras y puntos de progreso en líneas de progreso"
type: docs
weight: 3030
url: /es/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Representa la forma final en barras y puntos de progreso en líneas de progreso.

```csharp
public enum GanttBarEndShape
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| ArrowDown | `14` | Indica flecha apuntando hacia abajo Gantt bar end shape. |
| ArrowUp | `8` | Indica flecha apuntando hacia arriba Gantt bar end shape. |
| CaretDownTop | `9` | Indica caret apuntando hacia abajo en la mitad superior de la barra Gantt bar end shape. |
| CaretUpBottom | `10` | Indica caret apuntando hacia arriba en la mitad inferior de la barra Gantt bar end shape. |
| Circle | `19` | Indica círculo Gantt bar end shape. |
| CircleArrowDown | `18` | Indica flecha rodeada apuntando hacia abajo Gantt bar end shape. |
| CircleArrowUp | `17` | Indica flecha rodeada apuntando hacia arriba Gantt bar end shape. |
| CircleDiamond | `13` | Indica diamante rodeado Gantt bar end shape. |
| CircleTriangleDown | `16` | Indica triángulo rodeado apuntando hacia abajo Gantt bar end shape. |
| CircleTriangleUp | `15` | Indica triángulo rodeado apuntando hacia arriba Gantt bar end shape. |
| Diamond | `3` | Indica diamante Gantt bar end shape. |
| HouseDown | `2` | Indica casa invertida Gantt bar end shape. |
| HouseUp | `1` | Indica casa Gantt bar end shape. |
| LeftBracket | `21` | Indica corchete izquierdo Gantt bar end shape. |
| LeftFade | `23` | Indica desvanecimiento izquierdo Gantt bar end shape. |
| LineShape | `11` | Indica línea Gantt bar end shape. |
| NoBarEndShape | `0` | Indica ninguno Gantt bar end shape. |
| RightBracket | `22` | Indica corchete derecho Gantt bar end shape. |
| RightFade | `24` | Indica desvanecimiento derecho Gantt bar end shape. |
| Square | `12` | Indica cuadrado Gantt bar end shape. |
| Star | `20` | Indica estrella Gantt bar end shape. |
| TriangleDown | `5` | Indica triángulo apuntando hacia abajo Gantt bar end shape. |
| TriangleLeft | `7` | Indica la forma de triángulo que apunta a la izquierda al final de la barra de Gantt. |
| TriangleRight | `6` | Indica la forma de triángulo que apunta a la derecha al final de la barra de Gantt. |
| TriangleUp | `4` | Indica triángulo rodeado apuntando hacia arriba Gantt bar end shape. |

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

Muestra cómo usar estilos de barra personalizados en la vista del diagrama de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Los estilos de barra pueden ser específicos de tarea (ubicados en GanttChartView.CustomBarStyles).
// o específicos de categoría (ubicados en GanttChartView.BarStyles).
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Para fines de demostración, estamos modificando el estilo de la tarea con ID único = 4.
    // Aquí establecemos el campo (TaskName) para que se muestre a la izquierda de la barra de la tarea.
    ganttBarStyle.LeftField = Field.TaskName;
    // Aquí establecemos un convertidor personalizado para controlar qué texto se debe renderizar dentro de la barra de la tarea.
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

    // Para fines de demostración, estamos modificando los estilos aplicables a tareas de hito.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


