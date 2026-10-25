---
title: "Rsc.AvailableFrom"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La fecha de inicio en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual"
type: docs
weight: 120
url: /es/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

La fecha de inicio en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


