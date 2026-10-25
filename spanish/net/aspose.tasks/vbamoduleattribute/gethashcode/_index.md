---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaModuleAttribute. Devuelve un valor de código hash para este VbaModuleAttribute."
type: docs
weight: 40
url: /es/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Devuelve un valor de código hash para este [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

Devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de un atributo de módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// imprimir códigos hash de los atributos de un módulo VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Ver también

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


