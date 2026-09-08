---
title: "Asn.Summary"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of de taak een samenvattingstaak is"
type: docs
weight: 530
url: /nl/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

Bepaalt of de taak een samenvattende taak is.

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## Voorbeelden

Toont hoe de eigenschap Asn.Summary gelezen kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


