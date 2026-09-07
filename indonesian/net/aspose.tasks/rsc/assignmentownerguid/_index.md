---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. GUID dari pemilik penugasan"
type: docs
weight: 110
url: /id/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

GUID pemilik penugasan.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


