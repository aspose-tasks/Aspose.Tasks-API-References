---
title: "Asn.Created"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De datum waarop de toewijzing is gemaakt"
type: docs
weight: 210
url: /nl/net/aspose.tasks/asn/created/
---
## Asn.Created field

De datum waarop de opdracht is aangemaakt.

```csharp
public static readonly Key<DateTime, AsnKey> Created;
```

## Voorbeelden

Toont hoe de eigenschap Asn.Created gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Created, new DateTime(2020, 4, 9, 8, 0, 0));

Console.WriteLine("Created: " + assignment.Get(Asn.Created));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


