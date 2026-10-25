---
title: "Asn.LinkedFields"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si el proyecto está vinculado a otro objeto OLE"
type: docs
weight: 320
url: /es/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Determina si el Proyecto está vinculado a otro objeto OLE.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Ejemplos

Muestra cómo leer la propiedad Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


