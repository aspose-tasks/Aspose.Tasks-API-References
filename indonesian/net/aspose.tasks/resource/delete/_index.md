---
title: "Resource.Delete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Menghapus resource dan penugasannya dari proyek"
type: docs
weight: 810
url: /id/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Menghapus sebuah sumber daya dan penugasannya dari proyek.

```csharp
public void Delete()
```

## Contoh

Menampilkan cara menghapus resource.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// hapus resource
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Lihat Juga

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


