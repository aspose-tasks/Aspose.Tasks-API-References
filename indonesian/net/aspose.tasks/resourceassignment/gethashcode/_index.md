---
title: "ResourceAssignment.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Mengembalikan nilai kode hash untuk instance kelas ResourceAssignment"
type: docs
weight: 710
url: /id/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Mengembalikan nilai kode hash untuk instance dari kelas [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari penugasan sumber daya.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// cetak kode hash penugasan
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


