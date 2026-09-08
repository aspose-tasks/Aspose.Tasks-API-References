---
title: "ExtendedAttribute.ToString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttribute. Devuelve una representación corta en cadena de un atributo extendido"
type: docs
weight: 110
url: /es/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Devuelve la representación corta en cadena de un atributo extendido.

```csharp
public override string ToString()
```

### Valor devuelto

La representación en cadena del atributo extendido.

## Ejemplos

Muestra cómo leer atributos extendidos.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Leer atributos extendidos para tareas
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // Leer información común sobre el atributo extendido
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Ver también

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


