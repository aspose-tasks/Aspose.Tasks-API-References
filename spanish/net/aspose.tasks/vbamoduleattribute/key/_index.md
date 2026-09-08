---
title: "VbaModuleAttribute.Key"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaModuleAttribute. Obtiene la clave del atributo del módulo VBA"
type: docs
weight: 10
url: /es/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

Obtiene la clave del atributo del módulo VBA.

```csharp
public string Key { get; }
```

## Ejemplos

Muestra cómo trabajar con atributos de módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Ver también

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


