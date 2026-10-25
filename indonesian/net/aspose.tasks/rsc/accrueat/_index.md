---
title: "Rsc.AccrueAt"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menentukan bagaimana dan kapan biaya standar serta lembur sumber daya harus dibebankan atau diakumulasikan ke biaya sebuah tugas"
type: docs
weight: 10
url: /id/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Menentukan bagaimana dan kapan biaya standar dan lembur sumber daya harus dibebankan, atau diakumulasi, ke biaya sebuah tugas.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


