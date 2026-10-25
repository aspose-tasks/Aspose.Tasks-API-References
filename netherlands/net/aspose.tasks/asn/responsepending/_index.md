---
title: "Asn.ResponsePending"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of de reactie is ontvangen voor een TeamAssign-bericht"
type: docs
weight: 480
url: /nl/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

Bepaalt of de respons is ontvangen voor een TeamAssign‑bericht.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Voorbeelden

Toont hoe de eigenschap Asn.ResponsePending gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


