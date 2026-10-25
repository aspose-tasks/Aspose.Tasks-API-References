---
title: "Rsc.Phonetics"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Ejaan fonetik nama sumber daya. Hanya untuk penggunaan dengan bahasa Jepang"
type: docs
weight: 560
url: /id/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

Ejaan fonetik nama sumber daya. Hanya untuk penggunaan dengan bahasa Jepang.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


