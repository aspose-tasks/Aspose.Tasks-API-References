---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraReadOptions. Obtiene o establece el UID de un proyecto para leer de un archivo que contiene varios proyectos."
type: docs
weight: 30
url: /es/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Obtiene o establece el UID de un proyecto para leer de un archivo que contiene varios proyectos.

```csharp
public int ProjectUid { get; set; }
```

## Ejemplos

Muestra cómo leer un proyecto de un archivo Primavera XML o Primavera XER que contiene varios proyectos.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Devuelve el proyecto con UID especial.
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


