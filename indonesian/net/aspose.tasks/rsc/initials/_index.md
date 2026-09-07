---
title: "Rsc.Initials"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Inisial sebuah sumber daya"
type: docs
weight: 370
url: /id/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Inisial sumber daya.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


