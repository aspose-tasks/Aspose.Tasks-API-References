---
title: "Clase ProjectView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.ProjectView. Clase de vista de proyectos"
type: docs
weight: 3300
url: /es/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Clase de vista del proyecto

```csharp
public class ProjectView
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Inicializa una nueva instancia de la clase `ProjectView`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Obtiene las columnas de vista del proyecto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Incluye columnas de Uid, nombre de tarea, nombre de recurso, trabajo y asignación de duración. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Incluye columnas de id, indicadores, nombre, duración, inicio y fin de la tarea. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Incluye columnas de Uid, nombre de recurso, tipo, etiqueta de material, iniciales, grupo, unidades máximas, tarifa estándar, tarifa de horas extra, costo por uso, acumulado en, calendario base y código de recurso. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Incluye Uid, name, start, finish y columnas de recurso de trabajo. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Incluye id, indicators, name, duration, start, finish, predecessors y columnas de tarea de nombres de recurso. |

## Ejemplos

Muestra cómo guardar un proyecto con vista de asignación.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


