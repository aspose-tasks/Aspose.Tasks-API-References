---
title: "Enumeración GanttBarFillPattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. Un patrón de relleno de formas"
type: docs
weight: 3040
url: /es/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Patrón de relleno de una forma.

```csharp
public enum GanttBarFillPattern
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Hollow | `0` | Patrón hueco. |
| SolidFill | `1` | Patrón de relleno sólido. |
| LightFill | `2` | Patrón de relleno claro. |
| MediumFill | `3` | Patrón de relleno medio. |
| DarkFill | `4` | Patrón de relleno oscuro. |
| DiagonalLeft | `5` | Patrón diagonal izquierdo (de la esquina superior izquierda a la esquina inferior derecha). |
| DiagonalRight | `6` | Patrón diagonal derecho (de la esquina superior derecha a la esquina inferior izquierda). |
| DiagonalCross | `7` | Patrón diagonal cruzado. |
| LineVertical | `8` | Patrón de línea vertical. |
| LineHorizontal | `9` | Patrón de línea horizontal. |
| LineCross | `10` | Patrón de línea cruzada. |
| SolidFillWithDashedBorder | `11` | Patrón sólido con borde punteado. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


