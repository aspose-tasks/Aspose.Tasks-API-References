---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraReadOptions. Obtiene o establece una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse."
type: docs
weight: 20
url: /es/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Obtiene o establece una bandera que indica si se deben conservar los identificadores únicos originales de las entidades.

```csharp
public bool PreserveUids { get; set; }
```

## Ejemplos

Muestra cómo cargar un proyecto de Primavera con el Id especificado usando &lt;see cref=\"LoadOptions\" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// establecer opciones de lectura de Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// trabajar con el proyecto...
```

### Ver también

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


