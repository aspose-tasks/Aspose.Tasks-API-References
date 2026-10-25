---
title: "Resource.ParentProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan proyek induk untuk kontainer ini"
type: docs
weight: 600
url: /id/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Mendapatkan proyek induk untuk kontainer ini.

```csharp
public Project ParentProject { get; }
```

## Contoh

Menampilkan cara menggunakan proyek induk dari resource.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// set pekerjaan untuk resource dengan menggunakan tipe unit waktu kerja proyek default.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Lihat Juga

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


