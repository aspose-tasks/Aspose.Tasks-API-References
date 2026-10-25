---
title: "ProjectView.Columns"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectView. Obtiene las columnas de la vista del proyecto"
type: docs
weight: 70
url: /es/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

Obtiene las columnas de vista del proyecto.

```csharp
public List<ViewColumn> Columns { get; }
```

## Ejemplos

Muestra cómo guardar un proyecto con una vista con un conjunto personalizado de columnas.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// iterar sobre las columnas de la vista
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Ver también

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


