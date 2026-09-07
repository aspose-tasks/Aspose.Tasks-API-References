---
title: "Rsc.IsGeneric"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menentukan apakah sebuah sumber daya bersifat generik atau tidak"
type: docs
weight: 410
url: /id/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Menentukan apakah sumber daya bersifat umum atau tidak.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


