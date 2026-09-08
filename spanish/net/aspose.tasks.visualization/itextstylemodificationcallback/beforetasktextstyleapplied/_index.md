---
title: "ITextStyleModificationCallback.BeforeTaskTextStyleApplied"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ITextStyleModificationCallback. El método que se llamará antes de renderizar una celda de tabla para una fila de tarea en las siguientes vistas Gantt Chart Task Sheet Task Usage."
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/
---
## ITextStyleModificationCallback.BeforeTaskTextStyleApplied method

El método que se debe llamar antes de renderizar una celda de tabla para una fila de tarea en las siguientes vistas: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

```csharp
public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | TaskTextStyleEventArgs | El objeto [`TaskTextStyleEventArgs`](../../tasktextstyleeventargs/). |

## Ejemplos

Muestra cómo agregar columnas de vista para exportar.

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // iterar sobre columnas
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// El método que se debe llamar antes de renderizar una celda de tabla para una fila de tarea en las siguientes vistas:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">El objeto <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" />.</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### Ver también

* class [TaskTextStyleEventArgs](../../tasktextstyleeventargs/)
* interface [ITextStyleModificationCallback](../)
* namespace [Aspose.Tasks.Visualization](../../itextstylemodificationcallback/)
* assembly [Aspose.Tasks](../../../)


