---
title: "Rsc.IsNull"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Menentukan apakah sumber daya bernilai null"
type: docs
weight: 420
url: /id/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Menentukan apakah sumber daya bernilai null.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


