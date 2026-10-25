---
title: "Rsc.Name"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Nama sebuah sumber daya"
type: docs
weight: 460
url: /id/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Nama sumber daya.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


