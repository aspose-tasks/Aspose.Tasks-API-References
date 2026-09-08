---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "LoadOptions propiedad. Obtiene o establece una instancia especificada de la clase PrimaveraReadOptions que puede usarse para personalizar el comportamiento de carga de formatos Primavera Primavera P6 XER o Primavera P6 Xml"
type: docs
weight: 60
url: /es/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Obtiene o establece una instancia especificada de la clase [`PrimaveraReadOptions`](../../primaverareadoptions/) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


