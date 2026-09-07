---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menampilkan apakah sumber daya saat ini adalah sumber daya tim"
type: docs
weight: 430
url: /id/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Menampilkan apakah sumber daya saat ini adalah sumber daya tim.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


