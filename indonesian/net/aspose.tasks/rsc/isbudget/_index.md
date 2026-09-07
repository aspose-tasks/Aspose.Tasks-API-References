---
title: "Rsc.IsBudget"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menentukan apakah material kerja atau sumber daya biaya merupakan sumber daya anggaran"
type: docs
weight: 380
url: /id/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Menentukan apakah sumber daya kerja, material, atau biaya merupakan sumber daya anggaran.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


