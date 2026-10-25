---
title: "Rsc.Finish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La fecha en que se programa que un recurso complete el trabajo en todas las tareas asignadas"
type: docs
weight: 290
url: /es/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

La fecha en que se programa que un recurso complete el trabajo en todas las tareas asignadas.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


