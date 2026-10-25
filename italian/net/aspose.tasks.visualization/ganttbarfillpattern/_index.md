---
title: "Enum GanttBarFillPattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "**Aspose.Tasks.Visualization.GanttBarFillPattern** enum. Un modello di riempimento delle forme"
type: docs
weight: 3040
url: /it/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Modello di riempimento di una forma.

```csharp
public enum GanttBarFillPattern
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Hollow | `0` | Modello vuoto. |
| SolidFill | `1` | Modello di riempimento solido. |
| LightFill | `2` | Modello di riempimento chiaro. |
| MediumFill | `3` | Modello di riempimento medio. |
| DarkFill | `4` | Modello di riempimento scuro. |
| DiagonalLeft | `5` | Modello diagonale sinistro (dall'angolo superiore sinistro a quello inferiore destro). |
| DiagonalRight | `6` | Modello diagonale destro (dall'angolo superiore destro a quello inferiore sinistro). |
| DiagonalCross | `7` | Modello a croce diagonale. |
| LineVertical | `8` | Modello di linea verticale. |
| LineHorizontal | `9` | Modello di linea orizzontale. |
| LineCross | `10` | Modello di linea a croce. |
| SolidFillWithDashedBorder | `11` | Modello solido con bordo tratteggiato. |

## Esempi

Mostra come impostare gli stili di barra personalizzati della vista progetto del diagramma di Gantt.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Aggiungi lo stile di barra personalizzato alla collezione di barre personalizzate della vista progetto
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

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


