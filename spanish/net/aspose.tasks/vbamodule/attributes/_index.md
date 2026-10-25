---
title: "VbaModule.Attributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaModule. Obtiene una colección de los atributos del módulo"
type: docs
weight: 30
url: /es/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Obtiene una colección de los atributos del módulo.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Ejemplos

Muestra cómo leer los atributos del módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### Ver también

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


