---
title: "Resource.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Resource. Devuelve un valor de código hash para la instancia de la clase Resource"
type: docs
weight: 840
url: /es/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de un recurso.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// el código hash de un recurso es igual al UID del recurso 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Ver también

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


