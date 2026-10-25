---
title: "Asn.Uid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Το μοναδικό αναγνωριστικό μιας ανάθεσης"
type: docs
weight: 560
url: /el/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

Το μοναδικό αναγνωριστικό μιας ανάθεσης.

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.Uid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


