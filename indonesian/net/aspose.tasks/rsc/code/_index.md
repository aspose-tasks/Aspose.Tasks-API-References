---
title: "Rsc.Code"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Kode atau informasi lain tentang sumber daya"
type: docs
weight: 210
url: /id/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Kode atau informasi lain tentang sumber daya.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


