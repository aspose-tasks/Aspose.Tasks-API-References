---
title: "Rsc.ActualOvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Biaya yang timbul untuk pekerjaan lembur yang sudah dilakukan pada tugas oleh sumber daya yang ditugaskan"
type: docs
weight: 40
url: /id/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Biaya yang timbul untuk pekerjaan lembur yang sudah dilakukan pada tugas oleh sumber daya yang ditugaskan.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


