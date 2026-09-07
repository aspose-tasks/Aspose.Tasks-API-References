---
title: "Resource.Assignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan koleksi penugasan sumber daya untuk objek ini"
type: docs
weight: 120
url: /id/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Mendapatkan koleksi penugasan sumber daya untuk objek ini.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Contoh

Menampilkan cara membaca penugasan sumber daya.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### Lihat Juga

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


