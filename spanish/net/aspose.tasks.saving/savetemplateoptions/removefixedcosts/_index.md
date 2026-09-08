---
title: "SaveTemplateOptions.RemoveFixedCosts"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveTemplateOptions. Obtiene o establece un valor que indica si se deben eliminar todos los costos fijos de una plantilla de proyecto"
type: docs
weight: 40
url: /es/net/aspose.tasks.saving/savetemplateoptions/removefixedcosts/
---
## SaveTemplateOptions.RemoveFixedCosts property

Obtiene o establece un valor que indica si se deben eliminar todos los costos fijos de una plantilla de proyecto.

```csharp
public bool RemoveFixedCosts { get; set; }
```

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

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


