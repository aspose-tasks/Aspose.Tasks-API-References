---
title: "Resource.IsRoot"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Resource. Obtiene el indicador que muestra si el recurso es un recurso raíz. Un recurso raíz es un recurso especial que está destinado a soportar los internos de los formatos de MS Projects y no está destinado a ser usado directamente desde el código del usuario"
type: docs
weight: 470
url: /es/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Obtiene la bandera que indica si el recurso es un recurso raíz. El recurso raíz es un recurso especial que está destinado a soportar los internos de los formatos de MS Project y no está destinado a ser usado directamente desde el código del usuario.

```csharp
public virtual bool IsRoot { get; }
```

## Ejemplos

Muestra cómo usar la propiedad IsRoot para omitir el recurso raíz.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Ver también

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


