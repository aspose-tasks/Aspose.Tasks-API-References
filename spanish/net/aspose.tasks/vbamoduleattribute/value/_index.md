---
title: "VbaModuleAttribute.Value"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaModuleAttribute. Obtiene el valor del atributo del módulo VBA."
type: docs
weight: 20
url: /es/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Obtiene el valor del atributo del módulo VBA.

```csharp
public string Value { get; }
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


