---
title: "Rsc.Workgroup"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El tipo de grupo de trabajo al que pertenece un recurso"
type: docs
weight: 700
url: /es/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

El tipo de grupo de trabajo al que pertenece un recurso.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


