---
title: "Rsc.Start"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La fecha en que un recurso asignado está programado para comenzar a trabajar en una tarea"
type: docs
weight: 640
url: /es/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

La fecha en que un recurso asignado está programado para comenzar a trabajar en una tarea.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


