---
title: "Rsc.Id"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Pengidentifikasi posisi sebuah sumber daya dalam daftar sumber daya"
type: docs
weight: 350
url: /id/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

Pengidentifikasi posisi sumber daya dalam daftar sumber daya.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


