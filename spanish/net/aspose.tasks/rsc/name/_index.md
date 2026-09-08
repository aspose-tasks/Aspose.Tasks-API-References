---
title: "Rsc.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. El nombre de un recurso"
type: docs
weight: 460
url: /es/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

El nombre de un recurso.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


