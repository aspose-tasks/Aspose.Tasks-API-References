---
title: "Clase GanttChartColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.GanttChartColumn. Clase de vista de proyectos"
type: docs
weight: 3090
url: /es/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Clase de vista del proyecto

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Inicializa una nueva instancia de la clase GanttChartColumn. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Campo de columna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtiene el nombre de la columna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtiene o establece la alineación del texto (puede ser uno de los valores de la enumeración [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtiene o establece la devolución de llamada que puede usarse para personalizar la apariencia de las celdas de la columna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtiene el ancho de la columna. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Convierte la tarea actual al texto de la columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de diagrama de Gantt para exportar.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// iterar sobre columnas
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### Ver también

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


