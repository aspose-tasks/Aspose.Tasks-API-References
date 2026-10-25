---
title: "Asn.LinkedFields"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Determina se il Progetto è collegato a un altro oggetto OLE"
type: docs
weight: 320
url: /it/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Determina se il progetto è collegato a un altro oggetto OLE.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Esempi

Mostra come leggere la proprietà Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


