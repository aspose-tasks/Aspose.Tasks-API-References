---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectView. Incluye columnas de asignación Uid, nombre de tarea, nombre de recurso, trabajo y duración"
type: docs
weight: 20
url: /es/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Incluye columnas de Uid, nombre de tarea, nombre de recurso, trabajo y asignación de duración.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Valor devuelto

una vista que contiene una lista de [`AssignmentViewColumn`](../../assignmentviewcolumn/).

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


