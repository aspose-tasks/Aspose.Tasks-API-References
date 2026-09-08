---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Muestra si el recurso actual es un recurso de equipo"
type: docs
weight: 430
url: /es/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Muestra si el recurso actual es un recurso de equipo.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


