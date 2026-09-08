---
title: "MPPSaveOptions.ClearVba"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP."
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Obtiene o establece un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP.

```csharp
public bool ClearVba { get; set; }
```

## Ejemplos

Muestra cómo eliminar macros VBA de un archivo MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Ver también

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


