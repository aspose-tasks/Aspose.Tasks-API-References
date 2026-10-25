---
title: "Rsc.Code"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. El código u otra información sobre un recurso"
type: docs
weight: 210
url: /es/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

El código u otra información sobre un recurso.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


