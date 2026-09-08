---
title: "Estructura KeyTK"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Key2TK estructura. Representa una clave de propiedad de una clase del tipo especificado. Una instancia de esta clase se usa al obtener o establecer la propiedad de un contenedor."
type: docs
weight: 930
url: /es/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Representa una clave de propiedad de una clase del tipo especificado. Una instancia de esta clase se utiliza al obtener o establecer la propiedad de un contenedor.

```csharp
public struct Key<T, K>
    where K : struct
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo del valor de la propiedad. |
| K | El tipo de la clave de la propiedad. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Obtiene la clave de la propiedad. |

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


