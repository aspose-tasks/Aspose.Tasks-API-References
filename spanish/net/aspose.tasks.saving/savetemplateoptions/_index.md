---
title: "Clase SaveTemplateOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.SaveTemplateOptions. Permite especificar opciones adicionales al guardar un proyecto como plantilla"
type: docs
weight: 2200
url: /es/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Permite especificar opciones adicionales al guardar un proyecto como plantilla.

```csharp
public class SaveTemplateOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar todos los valores reales de una plantilla de proyecto. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar todos los valores de referencia de una plantilla de proyecto. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar todos los costos fijos de una plantilla de proyecto. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar las tarifas de recursos de una plantilla de proyecto. |

## Ejemplos

Muestra cómo guardar un proyecto como plantilla usando opciones.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// crear opciones de guardado de plantilla
// y ajustar sus propiedades
var options = new SaveTemplateOptions
{
    // establecer un valor que indique si se deben eliminar todos los costos fijos de una plantilla de proyecto
    RemoveFixedCosts = true,

    // establecer un valor que indique si se deben eliminar todos los valores reales de una plantilla de proyecto
    RemoveActualValues = true,

    // establecer un valor que indique si se deben eliminar las tarifas de recursos de una plantilla de proyecto
    RemoveResourceRates = true,

    // establecer un valor que indique si se deben eliminar todos los valores de referencia de una plantilla de proyecto
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


