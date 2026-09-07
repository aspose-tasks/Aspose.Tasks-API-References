---
title: "Asn.Milestone"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Menentukan apakah penugasan merupakan tonggak."
type: docs
weight: 330
url: /id/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Menentukan apakah penugasan adalah tonggak.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Contoh

Menampilkan cara membaca properti Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


