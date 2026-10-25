---
title: "Rsc.AssignmentOwner"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Nama pemilik penugasan"
type: docs
weight: 100
url: /id/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Nama pemilik penugasan.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


