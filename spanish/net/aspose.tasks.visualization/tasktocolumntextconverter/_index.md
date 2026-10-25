---
title: "Delegado TaskToColumnTextConverter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Convertidor de datos de tareas a cadena de columnas"
type: docs
weight: 3400
url: /es/net/aspose.tasks.visualization/tasktocolumntextconverter/
---
## TaskToColumnTextConverter delegate

Convertidor de datos de tarea a cadena de columna.

```csharp
public delegate string TaskToColumnTextConverter(Task task);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | Tarea actual. |

### Valor devuelto

Datos de cadena para la columna.

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


