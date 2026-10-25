---
title: "Project.DisplayOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene una instancia de la clase ProjectDisplayOptions"
type: docs
weight: 380
url: /es/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Obtiene una instancia de la clase [`ProjectDisplayOptions`](../../projectdisplayoptions/).

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Ejemplos

Muestra cómo ajustar las opciones de visualización del proyecto.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Establece un valor que indica si se deben mostrar advertencias cuando Project identifica un posible conflicto de programación con una tarea programada manualmente.
// Esta opción está disponible para la versión Project 2010 y posteriores.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Ver también

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


