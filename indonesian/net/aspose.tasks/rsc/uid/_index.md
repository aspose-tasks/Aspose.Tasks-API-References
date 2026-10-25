---
title: "Rsc.Uid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Pengidentifikasi unik dari sebuah sumber daya"
type: docs
weight: 670
url: /id/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

Pengidentifikasi unik sebuah sumber daya.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


