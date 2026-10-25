---
title: "Asn.LinkedFields"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Menentukan apakah Proyek terhubung ke objek OLE lain"
type: docs
weight: 320
url: /id/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Menentukan apakah Proyek terhubung ke objek OLE lain.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Contoh

Menampilkan cara membaca properti Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


