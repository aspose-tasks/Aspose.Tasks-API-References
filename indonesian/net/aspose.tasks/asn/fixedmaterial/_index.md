---
title: "Asn.FixedMaterial"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Menentukan apakah konsumsi sumber daya material yang ditugaskan terjadi dalam satu jumlah tetap"
type: docs
weight: 260
url: /id/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Menentukan apakah konsumsi sumber daya material yang ditugaskan terjadi dalam satu jumlah tetap.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Contoh

Menampilkan cara membaca/menulis properti Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


