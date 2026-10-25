---
title: "Rsc.CanLevel"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menentukan apakah penyeimbangan sumber daya dapat dilakukan pada sebuah sumber daya"
type: docs
weight: 200
url: /id/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Menentukan apakah perataan sumber daya dapat dilakukan pada sumber daya.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


