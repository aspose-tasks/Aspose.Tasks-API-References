---
title: "Rsc.Created"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Tanggal dan waktu ketika sebuah sumber daya ditambahkan ke proyek"
type: docs
weight: 260
url: /id/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

Tanggal dan waktu ketika sumber daya ditambahkan ke proyek.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


