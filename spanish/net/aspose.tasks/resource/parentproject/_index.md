---
title: "Resource.ParentProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Resource. Obtiene el proyecto principal para este contenedor"
type: docs
weight: 600
url: /es/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Obtiene el proyecto padre para este contenedor.

```csharp
public Project ParentProject { get; }
```

## Ejemplos

Muestra cómo usar el proyecto principal del recurso.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Establece un trabajo para el recurso usando el tipo de unidad de tiempo de trabajo predeterminado del proyecto.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Ver también

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


