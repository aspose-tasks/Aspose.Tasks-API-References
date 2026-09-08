---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraXmlSaveOptions. Obtiene o establece un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Obtiene o establece un valor que indica si se deben omitir las asignaciones de recursos a tareas resumidas durante la exportación.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Observaciones

El software Primavera no admite asignaciones de recursos a tareas resumen (WBS). Por lo tanto, la exportación de dichas asignaciones puede resultar en un archivo inválido según el modelo de Primavera. Si es verdadero, las asignaciones a tareas resumen se omiten durante la exportación. Si es falso (valor predeterminado), se lanzará una excepción si se encuentra una asignación a una tarea resumen durante la exportación.

## Ejemplos

Muestra cómo usar la bandera SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera no admite asignaciones de recursos a tareas resumen.
// Por lo tanto, exportar esas asignaciones al formato Primavera puede resultar en archivos que no pueden importarse a Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Ver también

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


