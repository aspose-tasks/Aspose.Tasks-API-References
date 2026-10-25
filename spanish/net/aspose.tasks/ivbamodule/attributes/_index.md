---
title: "IVbaModule.Attributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad IVbaModule. Obtiene una colección de VbaModuleAttributeCollection"
type: docs
weight: 10
url: /es/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Obtiene una colección de [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


