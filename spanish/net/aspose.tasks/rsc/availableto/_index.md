---
title: "Rsc.AvailableTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La fecha de finalización en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual"
type: docs
weight: 130
url: /es/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

La fecha de finalización en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


