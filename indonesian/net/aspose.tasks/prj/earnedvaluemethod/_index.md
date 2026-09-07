---
title: "Prj.EarnedValueMethod"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Metode default untuk menghitung nilai yang diperoleh"
type: docs
weight: 310
url: /id/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

Metode default untuk menghitung nilai yang diperoleh.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


