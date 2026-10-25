---
title: "Rsc.Guid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Berisi kode identifikasi unik yang dihasilkan untuk sumber daya"
type: docs
weight: 310
url: /id/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Berisi kode identifikasi unik yang dihasilkan untuk sumber daya.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


