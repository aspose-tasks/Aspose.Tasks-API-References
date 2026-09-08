---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El GUID de un propietario de asignación"
type: docs
weight: 110
url: /es/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

El GUID del propietario de la asignación.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


