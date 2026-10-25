---
title: "Clase PrimaveraReadOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.PrimaveraReadOptions. Permite especificar opciones adicionales al leer archivos Primavera Xml o Primavera Xer."
type: docs
weight: 1370
url: /es/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Permite especificar opciones adicionales al leer archivos Primavera XML o Primavera XER.

```csharp
public class PrimaveraReadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Inicializa una nueva instancia de la clase `PrimaveraReadOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Obtiene o establece una bandera que indica si se deben conservar los identificadores únicos originales de las entidades. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Obtiene o establece el UID de un proyecto para leer de un archivo que contiene varios proyectos. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Obtiene o establece una bandera que indica si los proyectos de línea base deben cargarse. El valor predeterminado es verdadero. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


