---
title: "Rsc.AvailableFrom"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tanggal mulai ketika sebuah sumber daya tersedia untuk bekerja pada unit yang ditentukan untuk periode waktu saat ini"
type: docs
weight: 120
url: /id/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

Tanggal mulai ketika sumber daya tersedia untuk bekerja pada unit yang ditentukan untuk periode waktu saat ini.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


