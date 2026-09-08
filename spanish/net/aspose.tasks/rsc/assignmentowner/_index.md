---
title: "Rsc.AssignmentOwner"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El nombre de un propietario de asignación"
type: docs
weight: 100
url: /es/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

El nombre del propietario de la asignación.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


