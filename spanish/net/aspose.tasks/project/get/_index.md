---
title: "Project.Get"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del proyecto. Devuelve el valor al que está asignada la propiedad en este contenedor"
type: docs
weight: 1080
url: /es/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Devuelve el valor al que la propiedad está asignada en este contenedor.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Prj`](../../prj/) para obtener la clave de la propiedad. |

### Valor devuelto

el valor al que la propiedad está asignada en este contenedor.

## Ejemplos

Muestra cómo verificar una versión del proyecto.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Mostrar versión del proyecto
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


