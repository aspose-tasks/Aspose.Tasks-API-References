---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraReadOptions. Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER."
type: docs
weight: 50
url: /es/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


