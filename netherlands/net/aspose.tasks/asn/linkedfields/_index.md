---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. Bepaalt of het project gekoppeld is aan een ander OLE-object"
type: docs
weight: 320
url: /nl/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Bepaalt of het project gekoppeld is aan een ander OLE-object.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Voorbeelden

Toont hoe de eigenschap Asn.LinkedFields gelezen kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


