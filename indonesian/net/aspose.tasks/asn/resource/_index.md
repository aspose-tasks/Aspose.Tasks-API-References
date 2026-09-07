---
title: "Asn.Resource"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Sumber daya yang ditugaskan ke sebuah tugas"
type: docs
weight: 470
url: /id/net/aspose.tasks/asn/resource/
---
## Asn.Resource field

Sumber daya yang ditetapkan untuk sebuah tugas.

```csharp
public static readonly Key<Resource, AsnKey> Resource;
```

## Contoh

Menampilkan cara membaca properti Asn.Task dan Asn.Resource.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Resource](../../resource/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


